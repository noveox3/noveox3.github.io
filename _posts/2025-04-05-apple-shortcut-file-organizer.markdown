---
layout: post
title: "Apple Shortcut for organizing Files"
category: "projects"
tags: [ "iOS", "Shortcuts", "macOS", "Files" ]
lang: 'en'
robots: 'NOINDEX'
---

## What?

It's a Shortcut that helps to save files in a somewhat organized way.

You can set a folder structure and each folder can have separate tags. It will save those files to your iCloud Drive: `/Shortcuts/File Organizer/Your Folder`

You can find the Shortcuts [here](#resources)

### Buggies?

It's possible that you might encounter bugs. Since it's just a Shortcut you can inspect how it is put together. You will quickly see a lot of workarounds that I implemented, just to get to the functionality that I wanted (especially list handing / menu handling). But good luck going through that spaghetti mess in the first place. I miss using an actual syntax after this ;;

Unfortunately I already discovered unsupported file types when accessing them directly via share-sheet (e.g. .procreate, .psd). My guess is that file-types handle differently when they're not on disk yet but idk.


> If you have to reset the config, just go to the File Organizer Folder and delete `0_config.json`.
> It should generate a new one when you open either Shortcut.

### So it is iOS / iPadOS / macOS only?

Yes.

## How to use the Shortcut(s)

There are 2 Shortcuts. One that will show up in your 'Share Sheet' and one to configure the File Organizer.

### Save with File Organizer

1. Select the file you want to save with the 'Share Sheet'.
2. Select the folder where you want to save the file to.
3. Select the tags you want to apply to your file name.

It will almost certainly ask you if you want to allow saving files from the current file-source.

Alternatively on macOS you can add the 'Save with File Organizer'-Shortcut to your Dock. You'll be able to drag and drop the file on the Icon and it should result with the same functionality.

Tags are just applied to the file name, there isn't a proper tag-system in place. But you can search for a tag with the Files App in the Directory you want and it will filter all files with that tag. At least this is how I use it.

### Configure File Organizer

Open the 'Configure File Organizer' Shortcut.

#### Folders

In the folder configuration you can configure folders and tags. Tags are bound to folders. So it can look something like this:

- Documents
    - draft
    - important
    - archive
    - ...
- Images
    - vacation
    - nature
    - food
    - ...
- ...

#### Settings

`Preserve the Original File Name`:

You can select to use the original file name or use the file hash. Using the file hash will make all file names the same length so that might be a neat thing if you prioritize using proper tags anyway. Plus obviously the same blob will result into the same file name (without the tags).

`Convert Images to HEIF`:

For some reason I had trouble with thumbnails in the Files App. Don't know why but png's don't generate thumbnails in that App. HEIF reliably does so plus it saves some space. Unfortunately at the cost of compatibility, but I'm sure there's a Shortcut out there that can mass-convert images back to pngs :))

`Default folder`:

If you're planning to only save files to one folder anyway, you can enable this default folder and select one of your configured folders. This way it should skip the folder selection when you open the Save Shortcut.

---

## Resources

`Save with File Organizer`: [Get Shortcut here](https://www.icloud.com/shortcuts/1cf2bb127f4f4106933915266d48e9c9)

`Configure File Organizer`: [Get Shortcut here](https://www.icloud.com/shortcuts/d51081c8e54c428fbd64fb46ab24e82b)


