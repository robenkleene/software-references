# OBS

## Tips

- You can lock any layer just by clicking the lock icon.

## Monitoring

You can monitor your mic by clicking the gear icon for the audio, choosing `Advanced Audio Properties`, and then choosing `Monitor and Output` under `Audio Monitoring`.

## Notes

- Use `⌘↩` when to accept a new scene name otherwise it won't save

## Audio

- You can capture computer audio by selecting "Loopback Audio" as the output source.
- To mute an audio source, click the speaker icon
- In order to have per scene control over audio sources, you need to disable `Mic/Auxiliary Audio` in `Preferences > Audio`.
- To make an external Mix sound good, add a `Noise Suppression` filter

### Levels

- Rule of thumb: Music high in the green, voice in the yellow, without ever peaking

### Ducking

To make the music level automatically reduce when talking.

1. Add a `Compressor` to filters
2. Set `Ratio: 10` or (`Ratio: 5`), `Threshold: -30`, `Attack: 2`, `Release: 650`, `Output Gain: 0`, `Sidechain: Mic`

## Screen

- To resize the screen in the OBS preview, right-click the screen preview and select "Transform > Fit to Screen".

## Adjustments

You can make adjustments, like adding a filter to adjust brightness, by right-clicking a source and selecting "Filters".

## Permissions

- **Input Monitoring**: For hot keys to work.

## Formats

- Record to `mkv`, because `mp4` requires a finalization process before the video file is usable, therefore, if there's a crash while recording, the video file might be unusable.
- `mkv` is not supported by Adobe Premiere or Final Cut Pro, so some work will be needed to edit these files in those applications. It appears to be possible by just changing the container without modifying the original audio and video tracks at all. The process is roughly to take the video track (with is probably `H.264`), and the audio track (`aac` or `mp3`), and put them in a new `mp4` container.
