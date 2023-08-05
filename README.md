# Defold Pixel Camera Extension
 
1. Change the render script in game.project Bootstrap to /pixel_camera/render/pixel.render

2. Choose the camera type by sending this message to the render script
	msg.post("@render:", "use_pixel_projection", {near = -10, far = 10, margin_min_w = 512, margin_min_h = 512, margin_x = 0, margin_y = 0.2})
	msg.post(URL_RENDER, MSG_USE_PIXEL_PROJECTION, {near = -10, far = 10, margin_min_w = 512, margin_min_h = 512, margin_x = 0, margin_y = 0.2})

3. Margin (optional)
	margin_min_w / margin_min_h : the minimum window size before adding the margin
	margin_x / margin_y : the total margin size in percent (include both sides margin, so margin_y = 0.2 -> 10% top + 10% left)
