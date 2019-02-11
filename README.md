# to test large file
Last login: Fri Feb  8 17:59:18 on ttys000
Pronobs-Retina-MacBook-Pro:~ whizphone$ brew
Example usage:
  brew search [TEXT|/REGEX/]
  brew info [FORMULA...]
  brew install FORMULA...
  brew update
  brew upgrade [FORMULA...]
  brew uninstall FORMULA...
  brew list [FORMULA...]

Troubleshooting:
  brew config
  brew doctor
  brew install --verbose --debug FORMULA

Contributing:
  brew create [URL [--no-fetch]]
  brew edit [FORMULA...]

Further help:
  brew commands
  brew help [COMMAND]
  man brew
  https://docs.brew.sh
Pronobs-Retina-MacBook-Pro:~ whizphone$ brew install git-lfs
Updating Homebrew...
^Z
[1]+  Stopped                 brew install git-lfs
Pronobs-Retina-MacBook-Pro:~ whizphone$ git lfs install
git: 'lfs' is not a git command. See 'git --help'.

The most similar command is
	log
Pronobs-Retina-MacBook-Pro:~ whizphone$ brew install git-lfs
Error: Another active Homebrew update process is already in progress.
Please wait for it to finish or terminate it to continue.
==> Downloading https://homebrew.bintray.com/bottles/git-lfs-2.6.1.mojave.bottle
######################################################################## 100.0%
==> Pouring git-lfs-2.6.1.mojave.bottle.tar.gz
==> Caveats
Update your git config to finish installation:

  # Update global git config
  $ git lfs install

  # Update system git config
  $ git lfs install --system
==> Summary
🍺  /usr/local/Cellar/git-lfs/2.6.1: 63 files, 9.9MB
==> `brew cleanup` has not been run in 30 days, running now...
Removing: /Users/whizphone/Library/Caches/Homebrew/autoconf--2.69.high_sierra.bottle.4.tar.gz... (871.2KB)
Removing: /Users/whizphone/Library/Caches/Homebrew/icu4c--62.1.high_sierra.bottle.tar.gz... (25.5MB)
Removing: /Users/whizphone/Library/Caches/Homebrew/mysql--8.0.12.high_sierra.bottle.tar.gz... (59.4MB)
Removing: /Users/whizphone/Library/Caches/Homebrew/openssl--1.0.2p.high_sierra.bottle.tar.gz... (3.7MB)
Removing: /Users/whizphone/Library/Caches/Homebrew/pkg-config--0.29.2.high_sierra.bottle.tar.gz... (235.8KB)
Removing: /Users/whizphone/Library/Caches/Homebrew/postgresql--10.5.high_sierra.bottle.1.tar.gz... (10.6MB)
Removing: /Users/whizphone/Library/Caches/Homebrew/rbenv--1.1.1.high_sierra.bottle.1.tar.gz... (18.6KB)
Removing: /Users/whizphone/Library/Caches/Homebrew/readline--7.0.5.high_sierra.bottle.tar.gz... (494KB)
Removing: /Users/whizphone/Library/Caches/Homebrew/ruby-build--20180822.tar.gz... (57.2KB)
Removing: /Users/whizphone/Library/Caches/Homebrew/ruby-build--20181106.tar.gz... (58.3KB)
Removing: /Users/whizphone/Library/Caches/Homebrew/sqlite--3.24.0.high_sierra.bottle.tar.gz... (1.7MB)
Removing: /Users/whizphone/Library/Caches/Homebrew/autoconf-2.69.tar.gz... (1.8MB)
Removing: /Users/whizphone/Library/Caches/Homebrew/pkg-config-0.29.1.tar.gz... (1.9MB)
Removing: /Users/whizphone/Library/Caches/Homebrew/linkage.db... (72KB)
Removing: /Users/whizphone/Library/Logs/Homebrew/pkg-config... (4 files, 840KB)
Removing: /Users/whizphone/Library/Logs/Homebrew/coreutils... (64B)
Removing: /Users/whizphone/Library/Logs/Homebrew/postgresql... (1.3KB)
Removing: /Users/whizphone/Library/Logs/Homebrew/icu4c... (64B)
Removing: /Users/whizphone/Library/Logs/Homebrew/readline... (64B)
Removing: /Users/whizphone/Library/Logs/Homebrew/carthage... (1.6MB)
Removing: /Users/whizphone/Library/Logs/Homebrew/ruby-build... (2 files, 179B)
Removing: /Users/whizphone/Library/Logs/Homebrew/sqlite... (64B)
Removing: /Users/whizphone/Library/Logs/Homebrew/mysql... (1021B)
Removing: /Users/whizphone/Library/Logs/Homebrew/autoconf... (4 files, 16.7KB)
Removing: /Users/whizphone/Library/Logs/Homebrew/openssl... (64B)
Removing: /Users/whizphone/Library/Logs/Homebrew/rbenv... (64B)
Pruned 1 symbolic links and 2 directories from /usr/local
Pronobs-Retina-MacBook-Pro:~ whizphone$ git lfs install
Git LFS initialized.
Pronobs-Retina-MacBook-Pro:~ whizphone$ git status
fatal: not a git repository (or any of the parent directories): .git
Pronobs-Retina-MacBook-Pro:~ whizphone$ mkdir lfs
Pronobs-Retina-MacBook-Pro:~ whizphone$ cd lfs
Pronobs-Retina-MacBook-Pro:lfs whizphone$ echo "# to test large file" >> README.md
Pronobs-Retina-MacBook-Pro:lfs whizphone$ git init
Initialized empty Git repository in /Users/whizphone/lfs/.git/
Pronobs-Retina-MacBook-Pro:lfs whizphone$ git add README.md
Pronobs-Retina-MacBook-Pro:lfs whizphone$ git commit -m "first commit"
[master (root-commit) f03ec92] first commit
 1 file changed, 1 insertion(+)
 create mode 100644 README.md
Pronobs-Retina-MacBook-Pro:lfs whizphone$ git remote add origin https://github.com/nikhildhavale/lfstest.git
Pronobs-Retina-MacBook-Pro:lfs whizphone$ git push -u origin master
remote: Permission to nikhildhavale/lfstest.git denied to nikhilwhizdhavale.
fatal: unable to access 'https://github.com/nikhildhavale/lfstest.git/': The requested URL returned error: 403
Pronobs-Retina-MacBook-Pro:lfs whizphone$ ssh
usage: ssh [-46AaCfGgKkMNnqsTtVvXxYy] [-B bind_interface]
           [-b bind_address] [-c cipher_spec] [-D [bind_address:]port]
           [-E log_file] [-e escape_char] [-F configfile] [-I pkcs11]
           [-i identity_file] [-J [user@]host[:port]] [-L address]
           [-l login_name] [-m mac_spec] [-O ctl_cmd] [-o option] [-p port]
           [-Q query_option] [-R address] [-S ctl_path] [-W host:port]
           [-w local_tun[:remote_tun]] destination [command]
Pronobs-Retina-MacBook-Pro:lfs whizphone$ ssh connect
ssh: Could not resolve hostname connect: nodename nor servname provided, or not known
Pronobs-Retina-MacBook-Pro:lfs whizphone$ git push -u origin master
Counting objects: 3, done.
Writing objects: 100% (3/3), 236 bytes | 236.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/nikhildhavale/lfstest.git
 * [new branch]      master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.
Pronobs-Retina-MacBook-Pro:lfs whizphone$ pwd
/Users/whizphone/lfs
Pronobs-Retina-MacBook-Pro:lfs whizphone$ git status
On branch master
Your branch is up to date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	GoogleCast.framework/

nothing added to commit but untracked files present (use "git add" to track)
Pronobs-Retina-MacBook-Pro:lfs whizphone$ git add .
Pronobs-Retina-MacBook-Pro:lfs whizphone$ git commit -m "add framework"
[master 5415751] add framework
 345 files changed, 11751 insertions(+)
 create mode 120000 GoogleCast.framework/GoogleCast
 create mode 120000 GoogleCast.framework/Headers
 create mode 120000 GoogleCast.framework/Modules
 create mode 120000 GoogleCast.framework/Resources
 create mode 100644 GoogleCast.framework/Versions/A/GoogleCast
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKApplicationMetadata.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKCastChannel.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKCastContext+UI.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKCastContext.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKCastOptions.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKCastSession.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKColor.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKCommon.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKDefines.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKDevice.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKDeviceManager.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKDeviceProvider+Protected.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKDeviceProvider.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKDeviceScanner.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKDiscoveryManager.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKError.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKFilterCriteria.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKFrameworkResources.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKGameManagerChannel.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKGameManagerResult.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKGameManagerState.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKGameplayState.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKGenericChannel.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKGlobalFlags.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKImage.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKJSONUtils.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKLaunchOptions.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKLobbyState.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKLogger.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKLoggerFilter.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKMediaCommon.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKMediaControlChannel.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKMediaInformation.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKMediaMetadata.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKMediaQueueItem.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKMediaStatus.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKMediaTextTrackStyle.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKMediaTrack.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKNSDictionary+TypedValueLookup.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKPlayerInfo.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKPlayerState.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKRemoteMediaClient.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKRequest.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKSenderApplicationInfo.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKSession+Protected.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKSession.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKSessionManager.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKSessionTraits.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKUIButton.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKUICastButton.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKUICastContainerViewController.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKUIDeviceVolumeController.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKUIImageCache.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKUIImageHints.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKUIImagePicker.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKUIMediaController.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKUIMediaTrackSelectionViewController.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKUIMiniMediaControlsViewController.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GCKUIUtils.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/GoogleCast.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/NSDictionary+GCKAdditions.h
 create mode 100644 GoogleCast.framework/Versions/A/Headers/NSTimer+GCKAdditions.h
 create mode 100644 GoogleCast.framework/Versions/A/Modules/module.modulemap
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Base.lproj/CastComponents.storyboardc/6is-ze-qoP-view-Vah-jq-ZgN.nib
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Base.lproj/CastComponents.storyboardc/9V7-ce-5KJ-view-WQF-my-40r.nib
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Base.lproj/CastComponents.storyboardc/C87-rF-Kff-view-Z93-bw-eCT.nib
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Base.lproj/CastComponents.storyboardc/CastContainer.nib
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Base.lproj/CastComponents.storyboardc/CastInstructions.nib
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Base.lproj/CastComponents.storyboardc/DeviceConnectionNavigation.nib
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Base.lproj/CastComponents.storyboardc/Info.plist
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Base.lproj/CastComponents.storyboardc/MediaTrackSelectionController.nib
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Base.lproj/CastComponents.storyboardc/MediaTrackSelectionNavigation.nib
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Base.lproj/CastComponents.storyboardc/MiniMediaControlsViewController.nib
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Base.lproj/CastComponents.storyboardc/a4H-bv-VbH-view-Xbz-9K-eDJ.nib
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Base.lproj/CastComponents.storyboardc/egs-hj-bEX-view-MTY-Nw-q8O.nib
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Base.lproj/CastComponents.storyboardc/mzQ-08-M2L-view-QcC-yO-nhF.nib
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Base.lproj/GCKGuestModePairingViewController.nib
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/audio_track@1x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/audio_track@2x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/audio_track@3x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/cast_off@1x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/cast_off@2x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/cast_off@3x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/cast_on0@1x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/cast_on0@2x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/cast_on0@3x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/cast_on1@1x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/cast_on1@2x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/cast_on1@3x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/cast_on2@1x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/cast_on2@2x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/cast_on2@3x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/cast_on@1x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/cast_on@2x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/cast_on@3x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/cling.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/closed_captions@1x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/closed_captions@2x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/closed_captions@3x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/hardware_generic@1x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/hardware_generic@2x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/hardware_generic@3x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/hardware_speaker@1x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/hardware_speaker@2x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/hardware_speaker@3x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/hardware_speaker_group@1x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/hardware_speaker_group@2x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/hardware_speaker_group@3x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/hardware_tv@1x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/hardware_tv@2x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/hardware_tv@3x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/media_next@1x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/media_next@2x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/media_next@3x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/media_pause@1x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/media_pause@2x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/media_pause@3x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/media_play@1x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/media_play@2x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/media_play@3x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/media_previous@1x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/media_previous@2x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/media_previous@3x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/media_stop@1x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/media_stop@2x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/media_stop@3x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/slider_thumb@1x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/slider_thumb@2x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/slider_thumb@3x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/volume0@1x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/volume0@2x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/volume0@3x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/volume1@1x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/volume1@2x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/volume1@3x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/volume2@1x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/volume2@2x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/volume2@3x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/volume3@1x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/volume3@2x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/Icons/volume3@3x.png
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/af.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/af.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/af.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/ar.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/ar.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/ar.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/bg.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/bg.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/bg.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/bn.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/bn.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/bn.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/ca.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/ca.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/ca.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/cs.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/cs.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/cs.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/da.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/da.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/da.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/de.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/de.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/de.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/el.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/el.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/el.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/en.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/en.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/en.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/en_GB.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/en_GB.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/en_GB.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/en_US.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/en_US.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/en_US.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/es.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/es.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/es.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/es_419.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/es_419.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/es_419.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/et.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/et.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/et.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/fa.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/fa.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/fa.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/fi.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/fi.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/fi.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/fil.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/fil.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/fil.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/fr.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/fr.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/fr.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/hi.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/hi.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/hi.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/hr.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/hr.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/hr.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/hu.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/hu.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/hu.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/hy.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/hy.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/hy.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/id.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/id.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/id.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/is.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/is.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/is.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/it.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/it.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/it.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/iw.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/iw.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/iw.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/ja.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/ja.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/ja.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/ka.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/ka.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/ka.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/km.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/km.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/km.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/ko.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/ko.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/ko.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/lo.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/lo.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/lo.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/lt.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/lt.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/lt.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/lv.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/lv.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/lv.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/mk.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/mk.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/mk.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/mn.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/mn.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/mn.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/mr.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/mr.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/mr.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/ms.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/ms.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/ms.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/my.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/my.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/my.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/ne.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/ne.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/ne.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/nl.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/nl.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/nl.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/no.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/no.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/no.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/pl.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/pl.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/pl.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/pt.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/pt.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/pt.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/pt_PT.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/pt_PT.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/pt_PT.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/ro.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/ro.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/ro.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/ru.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/ru.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/ru.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/si.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/si.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/si.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/sk.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/sk.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/sk.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/sl.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/sl.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/sl.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/sr.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/sr.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/sr.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/sv.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/sv.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/sv.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/sw.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/sw.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/sw.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/ta.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/ta.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/ta.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/th.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/th.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/th.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/tr.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/tr.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/tr.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/uk.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/uk.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/uk.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/vi.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/vi.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/vi.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/zh.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/zh.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/zh.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/zh_CN.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/zh_CN.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/zh_CN.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/zh_TW.lproj/CastComponents.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/zh_TW.lproj/GCKGuestModePairingViewController.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/GoogleCastResources.bundle/zh_TW.lproj/Localizable.strings
 create mode 100644 GoogleCast.framework/Versions/A/Resources/Info.plist
 create mode 100644 GoogleCast.framework/Versions/A/Resources/OpenSourceLicenses/dynamic_annotations.html
 create mode 100644 GoogleCast.framework/Versions/A/Resources/OpenSourceLicenses/eigen3.html
 create mode 100644 GoogleCast.framework/Versions/A/Resources/OpenSourceLicenses/grte.html
 create mode 100644 GoogleCast.framework/Versions/A/Resources/OpenSourceLicenses/icu.html
 create mode 100644 GoogleCast.framework/Versions/A/Resources/OpenSourceLicenses/kissfft.html
 create mode 100644 GoogleCast.framework/Versions/A/Resources/OpenSourceLicenses/libresample.html
 create mode 100644 GoogleCast.framework/Versions/A/Resources/OpenSourceLicenses/libunwind.html
 create mode 100644 GoogleCast.framework/Versions/A/Resources/OpenSourceLicenses/objective_c_google_toolbox_for_mac.html
 create mode 100644 GoogleCast.framework/Versions/A/Resources/OpenSourceLicenses/pcre.html
 create mode 100644 GoogleCast.framework/Versions/A/Resources/OpenSourceLicenses/re2.html
 create mode 100644 GoogleCast.framework/Versions/A/Resources/OpenSourceLicenses/stl.html
 create mode 100644 GoogleCast.framework/Versions/A/Resources/OpenSourceLicenses/tz.html
 create mode 100644 GoogleCast.framework/Versions/A/Resources/OpenSourceLicenses/utf.html
 create mode 100644 GoogleCast.framework/Versions/A/Resources/OpenSourceLicenses/zlib.html
 create mode 120000 GoogleCast.framework/Versions/Current
Pronobs-Retina-MacBook-Pro:lfs whizphone$ git commit -m "framework added"
On branch master
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
Pronobs-Retina-MacBook-Pro:lfs whizphone$ git push origin master
Counting objects: 410, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (404/404), done.
Writing objects: 100% (410/410), 90.80 MiB | 2.45 MiB/s, done.
Total 410 (delta 111), reused 0 (delta 0)
remote: Resolving deltas: 100% (111/111), done.
remote: error: GH001: Large files detected. You may want to try Git Large File Storage - https://git-lfs.github.com.
remote: error: Trace: b0d9e333ff66f0edfdcfc9c7ee69eb2c
remote: error: See http://git.io/iEPt8g for more information.
remote: error: File GoogleCast.framework/Versions/A/GoogleCast is 254.18 MB; this exceeds GitHub's file size limit of 100.00 MB
To https://github.com/nikhildhavale/lfstest.git
 ! [remote rejected] master -> master (pre-receive hook declined)
error: failed to push some refs to 'https://github.com/nikhildhavale/lfstest.git'
Pronobs-Retina-MacBook-Pro:lfs whizphone$ git lfs track "GoogleCast.framework"
Tracking "GoogleCast.framework"
Pronobs-Retina-MacBook-Pro:lfs whizphone$ git add .gitattributes
Pronobs-Retina-MacBook-Pro:lfs whizphone$ git add GoogleCast.framework
Pronobs-Retina-MacBook-Pro:lfs whizphone$ git commit -m "large file"
[master 9d49cb8] large file
 1 file changed, 1 insertion(+)
 create mode 100644 .gitattributes
Pronobs-Retina-MacBook-Pro:lfs whizphone$ git push origin master
Counting objects: 413, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (407/407), done.
Writing objects: 100% (413/413), 90.80 MiB | 1.92 MiB/s, done.
Total 413 (delta 110), reused 0 (delta 0)
remote: Resolving deltas: 100% (110/110), done.
remote: error: GH001: Large files detected. You may want to try Git Large File Storage - https://git-lfs.github.com.
remote: error: Trace: 356cdd43976ef7999114490d3db0a1b5
remote: error: See http://git.io/iEPt8g for more information.
remote: error: File GoogleCast.framework/Versions/A/GoogleCast is 254.18 MB; this exceeds GitHub's file size limit of 100.00 MB
To https://github.com/nikhildhavale/lfstest.git
 ! [remote rejected] master -> master (pre-receive hook declined)
error: failed to push some refs to 'https://github.com/nikhildhavale/lfstest.git'
Pronobs-Retina-MacBook-Pro:lfs whizphone$ git lfs track "GoogleCast.framework/Versions/A/GoogleCast"
Tracking "GoogleCast.framework/Versions/A/GoogleCast"
Pronobs-Retina-MacBook-Pro:lfs whizphone$ git add GoogleCast.framework/Versions/A/GoogleCast
Pronobs-Retina-MacBook-Pro:lfs whizphone$ git commit -m "test large file"
[master 3974c42] test large file
 1 file changed, 0 insertions(+), 0 deletions(-)
 rewrite GoogleCast.framework/Versions/A/GoogleCast (99%)
Pronobs-Retina-MacBook-Pro:lfs whizphone$ git push origin master
Uploading LFS objects: 100% (1/1), 266 MB | 1.3 MB/s, done                                                                                                   
Counting objects: 419, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (413/413), done.
Writing objects: 100% (419/419), 90.80 MiB | 1.79 MiB/s, done.
Total 419 (delta 112), reused 0 (delta 0)
remote: Resolving deltas: 100% (112/112), done.
remote: error: GH001: Large files detected. You may want to try Git Large File Storage - https://git-lfs.github.com.
remote: error: Trace: 3f11d1490f99e7fb7632ee91d4487fb8
remote: error: See http://git.io/iEPt8g for more information.
remote: error: File GoogleCast.framework/Versions/A/GoogleCast is 254.18 MB; this exceeds GitHub's file size limit of 100.00 MB
To https://github.com/nikhildhavale/lfstest.git
 ! [remote rejected] master -> master (pre-receive hook declined)
error: failed to push some refs to 'https://github.com/nikhildhavale/lfstest.git'
Pronobs-Retina-MacBook-Pro:lfs whizphone$ git lfs track "GoogleCast.framework/Versions/A/GoogleCast"
"GoogleCast.framework/Versions/A/GoogleCast" already supported
Pronobs-Retina-MacBook-Pro:lfs whizphone$ git add .gitattributes
Pronobs-Retina-MacBook-Pro:lfs whizphone$ git add GoogleCast.framework/Versions/A/GoogleCast
Pronobs-Retina-MacBook-Pro:lfs whizphone$ git commit -m "test large file2"
[master 9aba0c7] test large file2
 1 file changed, 1 insertion(+)
Pronobs-Retina-MacBook-Pro:lfs whizphone$ git push origin master
Uploading LFS objects: 100% (1/1), 266 MB | 0 B/s, done                                                                                                      
Counting objects: 422, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (416/416), done.
Writing objects: 100% (422/422), 90.80 MiB | 2.63 MiB/s, done.
Total 422 (delta 113), reused 0 (delta 0)
remote: Resolving deltas: 100% (113/113), done.
remote: error: GH001: Large files detected. You may want to try Git Large File Storage - https://git-lfs.github.com.
remote: error: Trace: e0fb06b1cfb721a7c9591176c64c1cda
remote: error: See http://git.io/iEPt8g for more information.
remote: error: File GoogleCast.framework/Versions/A/GoogleCast is 254.18 MB; this exceeds GitHub's file size limit of 100.00 MB
To https://github.com/nikhildhavale/lfstest.git
 ! [remote rejected] master -> master (pre-receive hook declined)
error: failed to push some refs to 'https://github.com/nikhildhavale/lfstest.git'
Pronobs-Retina-MacBook-Pro:lfs whizphone$ git lfs track **/GoogleCast
Tracking "GoogleCast.framework/GoogleCast"
Pronobs-Retina-MacBook-Pro:lfs whizphone$ git commit -m "test"
On branch master
Your branch is ahead of 'origin/master' by 4 commits.
  (use "git push" to publish your local commits)

Changes not staged for commit:
	modified:   .gitattributes

no changes added to commit
Pronobs-Retina-MacBook-Pro:lfs whizphone$ git add .
Pronobs-Retina-MacBook-Pro:lfs whizphone$ git commt -m "test"
git: 'commt' is not a git command. See 'git --help'.

The most similar command is
	commit
Pronobs-Retina-MacBook-Pro:lfs whizphone$ git commit -m "test"
[master ecc4588] test
 1 file changed, 1 insertion(+)
Pronobs-Retina-MacBook-Pro:lfs whizphone$ git push origin master
fatal: unable to access 'https://github.com/nikhildhavale/lfstest.git/': Could not resolve host: github.com
Pronobs-Retina-MacBook-Pro:lfs whizphone$ git push origin master
Uploading LFS objects: 100% (1/1), 266 MB | 0 B/s, done                                                                                                      
Counting objects: 425, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (419/419), done.
Writing objects: 100% (425/425), 90.80 MiB | 569.00 KiB/s, done.
Total 425 (delta 114), reused 0 (delta 0)
remote: Resolving deltas: 100% (114/114), done.
remote: error: GH001: Large files detected. You may want to try Git Large File Storage - https://git-lfs.github.com.
remote: error: Trace: eb4ed506085046352906fdda7b295bcd
remote: error: See http://git.io/iEPt8g for more information.
remote: error: File GoogleCast.framework/Versions/A/GoogleCast is 254.18 MB; this exceeds GitHub's file size limit of 100.00 MB
To https://github.com/nikhildhavale/lfstest.git
 ! [remote rejected] master -> master (pre-receive hook declined)
error: failed to push some refs to 'https://github.com/nikhildhavale/lfstest.git'
Pronobs-Retina-MacBook-Pro:lfs whizphone$ 
