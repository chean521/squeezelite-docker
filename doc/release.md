# Release History

## Releases

There is roughly a release for each set of entries on the same date of the following changelog.  
Minor changes, especially to the documentation only, are not necessarily included in a dedicated release.  
Older build might be dropped in order to save space on docker-hub and incur in limitations.

## Changelog

Date|Type|Description
:---|:---|:---
2023-03-11|Dropped buster as the arm/v6 version of the docker image is not available
2023-03-11|Dropped kinetic and jammy builds, as they don't include arm/v6 versions
2023-03-11|Workflow for regular versions now includes arm/v6 see [#179](https://github.com/GioF71/squeezelite-docker/issues/179)
2023-03-11|Workflow for sourceforge versions (for amd64, arm/v7 and arm64/v8)
2023-01-03|Update|Soureforge binaries version bump
2023-01-03|Documentation|`Release.md` cleanup
2022-12-27|Bug|Fixed issue [#168](https://github.com/GioF71/squeezelite-docker/issues/168)
2022-11-27|Improvement|User mode for alsa output
2022-11-26|Update|Soureforge binaries version bump
2022-11-25|Improvement|Allow mixer device and volume control in presets
2022-11-24|Improvement|All presets moved to `builtin-presets.conf`
2022-11-06|Bug|Launching non-existing binary when trying to show available outputs
2022-11-05|Improvement|Removed duplicate code
2022-11-05|Build|Ubuntu `jammy` is `stable`, `kinetic` is `latest`
2022-11-05|Build|Add support for ubuntu kinetic
2022-11-04|Build|Multistage build
2022-11-01|Update|Upgraded sourceforge binary for armhf to 1411
2022-10-24|Improvement|Updated GitHub action versions
2022-10-13|Feature|User-level systemd service for pulseaudio renamed to squeezelite-pulse
2022-10-07|Feature|Support for logging levels
2022-10-02|Build|Add apt proxy support
2022-10-02|Feature|Include both alsa and pulseaudio versions of squeezelite
2022-10-02|Feature|PulseAudio support introduced for sourceforge versions
2022-09-28|Build|Support for release, main, devel and feature tags
2022-09-28|Presets|Add new preset for Gustard U12 DDC
2022-09-28|Documentation|Fixed typos/Cleanup
2022-09-28|Documentation|Track (new) image tags
2022-09-28|Presets|Add new presets (Aune X12 & S6, Yulong D200, Peachtree DAC-iT)
2022-09-28|Build|Only from tags (reduce number of builds)
2022-09-28|Build|Build from main and devel branch only (no dates, no timestamps)
2022-09-28|Build|Support for building releases from a `release` branch by pushing a tag `release/<release-version>`.
2022-09-27|Feature|PulseAudio mode works with images tagged as `latest`
2022-09-27|HouseKeeping|Build process reviewed
2022-09-27|HouseKeeping|Created special tags dictionary
2022-09-27|HouseKeeping|Avoid tags with timestamps for devel and branch builds
2022-09-20|Documentation|Clarify PulseAudio mode instructions
2022-09-20|HouseKeeping|Add debian bookworm using v1.9.9. Images are tagged as `edge`
2022-09-20|HouseKeeping|Apply `latest` and `stable` tags to bullseye/N
2022-09-20|HouseKeeping|Apply `edge` tag to bookworm/N
2022-09-20|HouseKeeping|Apply `edge` tag to bookworm/N
2022-09-20|HouseKeeping|Apply `legacy` tag to buster/N
2022-09-20|HouseKeeping|Apply `sourceforge-legacy` tag to buster/Y
2022-09-17|Documentation|Fixed typo on PGID notes
2022-09-17|Documentation|Mentioned PulseAudio early in Why section
2022-09-17|Feature|Player name default is based on the hostname
2022-09-17|Improvement|PulseAudio systemd service now should wait for the network
2022-09-15|Documentation|More documentation for PulseAudio mode
2022-09-15|HouseKeeping|Fixed use of PUID and PGID
2022-09-15|Feature|Initial PulseAudio support
2022-09-15|Documentation|Fixed docker hub tag documentation
2022-09-13|HouseKeeping|Dropped buster on sourceforge
2022-09-13|HouseKeeping|Stable = bullseye on repos
2022-09-09|HouseKeeping|Routine build
2022-09-09|Documentation|Small corrections/typos
2022-08-05|HouseKeeping|Routine build
2022-06-11|HouseKeeping|Removed hard-coded base image versions
2022-06-11|Presets|Added some presets
2022-06-11|Documentation|Small corrections/typos
2022-06-10|Documentation|Corrected squeezelite version
2022-06-10|Documentation|Remove reference to focal
2022-06-10|HouseKeeping|Base image bump
2022-06-09|Feature|Add support for the visualizer `-v` switch
2022-04-30|HouseKeeping|Arm 32bit client updated to version 1401
2022-04-30|HouseKeeping|Base image bump
2022-04-30|HouseKeeping|Upgraded to ubuntu jammy
2022-04-01|Documentation|Tinkerboard issue apparently solved
2022-03-29|Documentation|Small corrections/typos
2022-03-19|Presets|Add preset for Raspberry Pi Headphone out
2022-03-19|Documentation|Small corrections/typos
2022-03-14|Documentation|Testing documentation
2022-03-14|Documentation|Tinkerboard issue tracked
2022-03-14|HouseKeeping|Previously quarantined files removed
2022-03-12|HouseKeeping|Base image bump
2022-03-12|HouseKeeping|Binaries quarantined to `old/bin`
2022-02-04|Automation|Created Action for README.md synchronization
2022-02-04|Documentation|Release history moved out of README.md
2022-02-04|Documentation|Created `RELEASE.md` file
2022-02-23|Improvement|Packages upgrade during image build phase
2022-02-23|Feature|Add support for volume control: `-V` switch
2022-02-23|Feature|Add support for the unmute: `-U` switch
2022-02-23|Feature|Add support for linear volume: `-X` switch
2022-02-16|Improvement|Reviewed the presets loading mechanism
2022-02-16|Feature|Add DISPLAY_PRESETS env variable
2022-02-16|Feature|Allow custom preset files through volume
2022-02-14|Documentation|Reviewed the preset table layout
2022-02-14|Automation|Synchronization of `README.md` with [docker hub](https://hub.docker.com/r/giof71/squeezelite)
2022-02-14|Improvement|Focal tag is now `focal`
2022-02-14|Feature|Added preset `no-dsd`
2022-02-14|Feature|Added support for excluded codecs: `-e` switch
2022-02-05|Improvement|Automated builds thanks to [Der-Henning](https://github.com/Der-Henning/)
2022-02-05|Improvement|New builds for arm64 thanks to [Der-Henning](https://github.com/Der-Henning/)
2022-02-05|Improvement|`README.md` added to image
2022-02-04|Improvement|Simplified build process
2022-02-04|Improvement|Reduced image sizes
2022-02-04|Documentation|Documented the convenience build.sh script
2022-02-04|Automation|Corrected sourceforge tag names
2022-02-02|Feature|Allowed combination of presets
2022-02-02|Bugfix|Fixed incorrect mapping for SQUEEZELITE_DELAY
2022-02-02|Feature|Added `extremus` upsample setting
2022-02-02|Feature|Rate presets defined
2022-01-30|Feature|Added images with SourceForge binaries
2022-01-30|Feature|Long variable shortened