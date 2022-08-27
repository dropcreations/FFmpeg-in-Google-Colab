# __FFmpeg-for-Google-Colab__

Install latest __FFmpeg__ to the __Google Colab__ runtime.

<a href="https://colab.research.google.com/github/dropcreations/FFmpeg-for-Google-Colab/blob/main/FFmpeg-in-Google-Drive.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Colab"/></a>

- Click on the __"Open in Colab"__ button to open this notebook in google colab

# __Table of Contents__

- FFmpeg in Google Colaboratory

## <img width=25 alt="Google-Drive-Logo" src=https://raw.githubusercontent.com/dropcreations/FFmpeg-for-Google-Colab/e19fd94a5bb7a1003fd433daaa796beafe5e2bd6/Google-Drive-Logo.svg> __Mount Google Drive__
- Mount your google drive to access it's files in colab

## <img width=20 alt="FFmpeg-Logo" src=https://raw.githubusercontent.com/dropcreations/FFmpeg-for-Google-Colab/32abf44ff4c8d145a94a24611f01141926a8daaa/FFmpeg-Logo.svg></img> __FFmpeg__
- Install FFmpeg

### __Remux Video Files__
* **REMUX** video files without **RE-ENCODING**.
* Make sure that `outputFormat` that you have selected is supported for all tracks in the `inputFile`.
* `WebM` only support `VP9`, `VP8`, `AV1` video and `Vorbis`, `Opus` audio and `WebVTT` subtitles.
### __Trim Video Files__
* **TRIM** video files without **RE-ENCODING**.
* `inputFile`: video file's path and set `startTime` and `endTime` to trim.
* Trimed video will be saved as same as the **source's format**.
### __Extract Audio__
* **EXTRACT** audio tracks from video files.
* `DTS`, `DTS-HD`, `DTS-MA`, `TrueHD` tracks will be muxed as a `.mka` file.
### __Remove Bitstream Metadata__
* For `H.264`/`AVC` tracks run first cell.
* For `H.265`/`HEVC` tracks run second cell.
### __Encode H.264__
* `CRF` and `2-Pass` encoding available.
* This cell only encodes the **first video track** from the input file.
### __HDR to SDR__
* Convert `HDR` video to `SDR` video.
* `toneMap`: Select tone mapping method.
### __HDR10 Encoding__
* Only `x265`/`HEVC` tracks are supported.
* `extractColors`: View the color information of the footage.
* When encoding, make sure `extractColors` is **deselected**.
