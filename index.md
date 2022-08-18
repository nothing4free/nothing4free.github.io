---
layout: home
title: /
permalink: /
---

### hack the planet and listen to techno!

this website is under construction, please wait...

<script>
    var w = c.width = window.innerWidth,
		h = c.height = window.innerHeight,
		ctx = c.getContext( '2d' ),
		
		opts = {
			boldnessProbability: .01,
			fontSize: 12,
			fontSpacing: 12,
			fontFamily: 'monospace',
			charAdded: 1, // par frame
			charset: '                                                                                                                          `1234567890-=¬!"£$%^&*()_+qwertyuiop[]QWERTYUIOP{}asdfghjkl;\'#ASDFGHJKL:@~\\zxcvbnm,./|ZXCVBNM<>?', // yes, a lot of spaces
			rainbowXMultiplier: .5,
			rainbowYMultiplier: .5,
			rainbowXSpeed: 10,
			rainbowYSpeed: 1.2
		},
		
		charsToAdd = 0,
		tickX = 0,
		tickY = 0,
		text = [];

function anim(){
	
	window.requestAnimationFrame( anim );
	
	ctx.fillStyle = 'black';
	ctx.fillRect( 0, 0, w, h );
	
	charsToAdd += opts.charAdded;
	
	tickX += opts.rainbowXSpeed;
	tickY += opts.rainbowYSpeed;
	
	ctx.font = opts.fontSize + 'px ' + opts.fontFamily;
	
	while( charsToAdd > 0 ){
		--charsToAdd
		text.pop();
		text.unshift( opts.charset[ ( Math.random() * opts.charset.length ) |0 ] );
	}
	
	var n = 0;
	for( var i = 0; i < w; i += opts.fontSpacing ){
		
		var rainbowXFactor = i * opts.rainbowXMultiplier;
		
		for( var j = 0; j < h; j += opts.fontSpacing ){
			
			++n;
			var char = text[ n ];
			
			if( char ){
				
				if( char !== ''){
					
					ctx.fillStyle = 'hsl(hue,80%,50%)'
						.replace( 'hue', 
										 rainbowXFactor + tickX
										 + j * opts.rainbowYMultiplier + tickY );
					ctx.fillText( text[ n ], i, j );
				}
			} else {
				i = w;
				j = h;
			}
		}
	}
}

function setup(){
	
	text.length = 0;
	
	var num = ( ( w / opts.fontSpacing + 1 ) |0 ) * ( ( h / opts.fontSpacing + 1 ) |0 );
	
	while( --num )
		text.push( opts.charset[ ( Math.random() * opts.charset.length ) |0 ] );
}

setup(); // just checking things in the debugger
anim();

window.addEventListener( 'resize', function(){
	
	w = c.width = window.innerWidth;
	h = c.height = window.innerHeight;
	
	setup();
})
</script>

<canvas id=c style="position: absolute; top: 0; left: 0;"></canvas>