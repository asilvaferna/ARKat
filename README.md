# ARKat

A simple AR Pet using Apple AR Kit plugin on Unity

## Getting started

If you want to use the AR Kit plugin on your project you must follow this step-by-step guide

### Prerequisites

- iOS Device with a A8 chip or best
- Macinstosh device with Xcode 9 installed
- Unity

### Installation

1. Open Unity on your device and download the [AR Kit Plugin](https://www.assetstore.unity3d.com/en/#!/content/92515)
2. Once donwloaded, import the files off the plugin
3. You are ready to go!


## Getting deeper

I have the plugin installed but, now what?

### The assets

When you have all the files imported, you must think, how do I do something with this? Well, we are on our way

First of all navigate through the folders and find the one called `/Examples/UnityARKitScene` double click on the asset **UnityARKitScene**.
You must see something like this: 

![GameObject](https://user-images.githubusercontent.com/22442331/32144053-4da596a4-bcb3-11e7-8393-5e81536f44b0.png)

### Understanding the game objects

The image on top ilustrates the current scene. Currently this game will just place one cube wherever you touch the screen. But wouldn't it be cooler that you could change that "ugly" cube and place instead one 3D object? In this example you will use the [Cartoon Cat](https://www.assetstore.unity3d.com/en/#!/content/70180) asset that can be found on the Asset Store.

- Replace the `HitCube` gameobject for one of the 3D models in the Cartoon Cat asset
- Delete `RandomCube` gameobject
- In the assets folder search for `shadowPlanePrefab` and add it to the Scene
- On `CameraParent` reset the axis to `x:0, y:0, z:0`. Do the same with `HitCubeParent` gameobject, and `shadowPlanePrefab`

After doing the instructions on top, the scene must be something like this:

![LastScene](https://user-images.githubusercontent.com/22442331/32145234-51e57dbc-bcc5-11e7-8afa-3a763ed106bb.png)

Then you just have to build the game with:  ⇧ + ⌘ + B

Keep reading to learn how to build the project in *Xcode*

### Xcode project building

Open *Xcode* and search the path of the builded unity game. In my case is `/Unity/AR Test/Builds`

Once opened, you have to modify the `Unity-iPhone` build file. Change the name of the app on `Display Name`, and the bundle identifier.
You have to sign the app with your Developer account. Change the Deployment Target to `iOS 11.0`.
Device orientation has to be like this:

- [x] Portrait
- [ ] Upside Down
- [x] Landscape Left
- [x] Landscape Right 

And you have finish! Make sure your iOS Device is plugged in, and click play button to build the project.

## Demo

<p align="center">
  <img src="https://user-images.githubusercontent.com/22442331/32146674-3b3d45d4-bcdb-11e7-98c6-a08e5ce4b8ee.gif" alt="Gif"/>
</p>

## Acknowledgments

- [Unity AR Kit Plugin reference](https://www.assetstore.unity3d.com/en/#!/content/92515)
- [YouTube tutorial](https://www.youtube.com/watch?v=EbbpAMr9JL4)
- Previous experience building Xcode apps


