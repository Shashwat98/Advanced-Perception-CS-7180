
# LIME (Low-Light Image Enhancement)

## Quick start
```bash
pip install numpy scipy scikit-image opencv-python
python lime_lite.py --input /path/to/dark.jpg --alpha 0.15 --gamma 0.8 --denoise nlmeans --save_maps
```

## Notes
- The refinement uses a single sparse linear system solve with weights from gradients of T_hat (per-pixel maxRGB).
- For batches with same image size, you could factorize the system once (not included in this minimal script).
- Selective denoising recomposes: R * T + R_denoised * (1 - T).
``

# Zero-DCE++
This can be referred at the official github repo: https://github.com/Li-Chongyi/Zero-DCE_extension/tree/main

python lowlight_test.py

The script will process the images in the sub-folders of "test-data" folder and make a new folder "result"
