---
layout: null
---

<html>
<head>
	<meta name="viewport" content="width=device-width, initial-scale=1">
	<style>
		* {
		  box-sizing: border-box;
		  margin: 0;
		  padding: 0;
		}

		.container {
		  position: relative;
		  width: 100%;
		}

		.image {
		  display: block;
		  width: 100%;
		  height: 100%;
		}

		.overlay {
		  position: absolute; 
		  bottom: 0; 
		  background: rgb(0, 0, 0);
		  background: rgba(0, 0, 0, 0.5); /* Black see-through */
		  color: #f1f1f1; 
		  width: 100%;
		  transition: .5s ease;
		  opacity:0;
		  color: white;
		  font-size: 20px;
		  padding: 20px;
		  text-align: center;
		}

		.derp {
			position: absolute;
			top: 0;
			right: 0;
			width: 150px;
			height: 150px;
			color: white;
			font-size: 20px;
			text-align: center;
		}

		.container:hover .overlay {
		  opacity: 1;
		}
	</style>
</head>
<body>
	<div class="container">
		<iframe class="image" width="100%" height="100%" src="https://www.youtube-nocookie.com/embed/TRgqtaYb4sU?si=qnPdzqwP_N2ReSDg&amp;controls=0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
		<div class="overlay">
			<p>Jarrod</p>
		</div>
		<div class="derp">
			<p>DERP</p>
		</div>
	</div>
</body>
</html>