# aerosol_disperions_wind_instruments
This document describes the structure of raw data about the aerosol disperion of wind instruments. The data include the pixel coordinates of the cloud contours in each frame for each player, task and perspective.

Data content:
- 3 trumpet, 3 cross flute and 3 clarinet players
- 3 tasks Mh-, Mh+ and Ml-
- 2 camera perspectives K1 (side view) and K3 (top view)
- Example:
	trumpet_1_Mh-_K1.snake		# trumpet player 1, task Mh-, K1 perspective (side view)

Data format:
- Ascii data, space separated
- Header: Length of data file, i.e. total number of frames in the file.
- Data field: Number of point coordinates describing the cloud contour in the respective frame followed by the coordinates (x,y) of each point.
- Example:
	
	Length		# Header
	155			# Header

	24			# Number of points describing the cloud contour
	546	405		# x- and y- coordinate in pixels
	545	405
	544	406
	544	407
	545	408
	546	409
	547	410
	547	411
	548	412
	549	413
	550	414
	551	414
	551	414
	552	413
	553	412
	553	411
	553	410
	552	409
	551	410
	550	409
	549	408
	548	407
	547	406
	546	405
	
	30			# Next frame
	547	404
	546	405
	545	406
	546	407
	547	408
	547	409
	547	410
	...	
	
