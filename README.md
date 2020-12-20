# AFrameAR
A simple AR project using A-Frame. AR.js is a lightweight library for Augmented Reality on the Web, coming with features like Image Tracking, Location-based AR and Marker tracking.
You can find the official library here: https://github.com/AR-js-org/AR.js

# AR Magic

Our project uses 2 GLTF models and a few presets. To test it just go to:
https://jojo96.github.io/AFrameAR/

Scan this marker:

<img src="https://github.com/jojo96/AFrameAR/blob/main/hiro.png"  alt="Normal">


You can see something like this:

<img src="https://github.com/jojo96/AFrameAR/blob/main/AR%20GIF.gif"  alt="Normal">

# Marker based AR

Marker-based augmented reality experiences require a static image also referred to as a trigger photo that a person can scan using their mobile device via an augmented reality app.


The skeleton code for our AR app is:
	
    <html>
    script src="https://aframe.io/releases/1.0.0/aframe.min.js"></script>
	<script src="./resources/animation-mixer.js"></script>
	<script src="https://unpkg.com/aframe-animation-component@5.1.2/dist/aframe-animation-component.min.js"></script>
    <!-- we import arjs version without NFT but with marker + location based support -->
    <script src="https://raw.githack.com/AR-js-org/AR.js/master/aframe/build/aframe-ar.js"></script>
    <body style="margin : 0px; overflow: hidden;">
        <a-scene embedded arjs>
       
       <a-marker preset="hiro">
		
        </a-marker>
        <a-entity camera></a-entity>
        </a-scene>
    </body>	
    </html>


You should add your code between the a-marker tags.






