# Harakat model packs

On-device speech models used by the Harakat iOS app (Arabic lyric videos). The app downloads these files
on first use and verifies each one against a SHA-256 and byte size compiled into the app. A file that doesn't
match is rejected. Audio never leaves the phone; these files are only the models.

Release **`harakat-models-v1`**:

| File | Size | Model | Licence |
|---|---|---|---|
| `omni-ctc300m-int8-v1.onnx` + `omni-ctc300m-tokens-v1.txt` | 365 MB | omniASR CTC-300M by Meta (int8 ONNX export via sherpa-onnx) | Apache-2.0 (`Apache-2.0.txt`, `omniASR-NOTICE.txt`) |
| `nvidia-ar-fc-ctc-int8-v1.onnx` + `nvidia-ar-fc-ctc-tokens-v1.txt` | 174 MB | Arabic FastConformer by NVIDIA (int8 ONNX export via sherpa-onnx) | CC BY 4.0 (`NVIDIA-FastConformer-CC-BY-4.0.txt`) |

Arabic FastConformer by NVIDIA, CC BY 4.0 (https://creativecommons.org/licenses/by/4.0/). Modified: int8 quantised, ONNX export.

Checksums: `SHA256SUMS`. Files are never replaced in place; a new version gets a new release tag.
