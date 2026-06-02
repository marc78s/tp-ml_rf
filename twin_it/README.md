# Files description
Resources for the *Twin it!* practice sessions.

Author: Joseph Chazalon, EPITA/LRDE, MLRF course

Date: 20200429-122000

All artwork is copyrighted by the original author, Thomas Vuarchex.

## Useful for all sessions
- `/bubbles_200dpi`: directory containing all extracted bubbles,
  at 200 dpi resolution, with appropriate masking.
- `README.md`: This file.
- `mask_bubbles.png`: Mask image of the bubbles vs background at 200 dpi.
- `twin_it_12dpi.jpg`: Poster image at 12 dpi.
- `twin_it_200dpi.png`: Poster image at 200 dpi.
- `twin_it_50dpi.png`: Poster image at 50 dpi.


## Useful for session 1 (Template matching)
- `dist_mat_sqdiff_normed.npz`: Triangular matrix of the sum of squared differences
between each pair of patches.


## Useful for session 2 (Color histograms, Harris corner detector, local descriptors, matching)
- `bubble_dist_mat_hsv7-cosine.npz`: NumPy export of: 1) the color histogram for each bubble (HSV color space, 7 colors) and 2) the square distance matrix computed between each histogram pair using the cosine distance.
- `bubble_dist_mat_rgb7-cosine.npz`: NumPy export of: 1) the color histogram for each bubble (RGB color space, 7 colors) and 2) the square distance matrix computed between each histogram pair using the cosine distance.
- `kpts_descr_harris_25pxcolor_mdist10.npz`: NumPy export of: 1) the coordinates of the corners detected using the Harris method (Noble's variant) and 2) the descriptors extracted around those keypoints. Parameters: min. 10 pixels between keypoints, descriptor size = 25x25 px, color patch
- `kpts_descr_harris_25pxcolor_mdist13.npz`: Same content. Parameters: min. 13 pixels between keypoints, descriptor size = 25x25 px, color patch
- `kpts_descr_harris_51pxcolor_mdist10.npz`: Same content. Parameters: min. 10 pixels between keypoints, descriptor size = 51x51 px, color patch
- `kpts_descr_harris_51pxcolor_mdist26.npz`: Same content. Parameters: min. 26 pixels between keypoints, descriptor size = 51x51 px, color patch


## Bonuses
- `bubbles_labels_stats.npz`: NumPy export of the label map (connected components)
  of all bubbles and the statistics for each, computed with OpenCV.


## Other resources
Course material (lectures and practice sessions) available here:
https://www.lrde.epita.fr/~jchazalo/teaching/MLRF/
