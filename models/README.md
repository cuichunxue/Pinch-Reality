# Models

| File | Source | License |
| --- | --- | --- |
| `animegan_hayao.onnx` | AnimeGANv2 Hayao (TachibanaYoshino), ONNX from npm `sts-animegan@1.0.0` | Academic / personal use only — no commercial use |
| `face_paint_v2.onnx` | animegan2-pytorch `face_paint_512_v2` (bryandlee), ONNX from npm `sts-animegan@1.0.0` | MIT |

`face_paint_v2.onnx` was patched to accept any input size: the constant shapes of the
GroupNorm reshapes were replaced with `Shape()` of the input tensor, and the two fixed-size
`Resize` nodes were changed to 2× scales.
