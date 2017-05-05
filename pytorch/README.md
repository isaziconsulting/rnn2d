# Prerequisits

* Install the PyTorch binding for Baidu's Warp-CTC implementation from [here](https://github.com/SeanNaren/warp-ctc/tree/pytorch_bindings/pytorch_binding)
    * If you come across the error "ImportError: No module named 'warpctc_pytorch._warp_ctc'" we fixed this by doing the following:
        * `rm /usr/local/lib/python3.5/dist-packages/torch/lib/libgomp.so.1`
        * `ln -s /usr/lib/x86_64-linux-gnu/libgomp.so.1 /usr/local/lib/python3.5/dist-packages/torch/lib/libgomp.so.1`
