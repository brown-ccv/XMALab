# XMA Lab

XMALab is software for marker-based fluoromicrometry and XROMM, with tools for standard (non-X-ray) video analysis as well. The developer is Dr. Ben Knorlein, a computer-vision expert and software engineer at the Center for Computation and Visualization at Brown University. XMALab has been described and validated in [a peer-reviewed paper](http://jeb.biologists.org/content/early/2016/09/21/jeb.145383) in the _Journal of Experimental Biology_.

XMALab integrates distortion correction, calibration, marker tracking, rigid body calculations and filtering all into one program. XMALab replaces all components of the MATLAB X-ray Project workflow. For marker-based XROMM, XMALab generates animation matrices suitable for animating bones in Autodesk Maya. XMALab also includes tools, such as checkerboard calibration, for motion analysis with standard (non-Xray) video.

Join the [XMALab Google Group](https://groups.google.com/a/brown.edu/forum/?hl=en#!forum/xmalab) to be notified of future releases and pose questions to the group.

XMALab development is supported by the US National Science Foundation through an Advances in Biological Informatics grant to PI Elizabeth Brainerd and CoPIs Stephen Gatesy and David Baier.

***

## Development

From your terminal:

```sh
npm run dev
```

This starts your app in development mode, rebuilding assets on file changes.

## Deployment

First, build your app for production:

```sh
npm run build
```

Then run the app in production mode:

```sh
npm start
```

Now you'll need to pick a host to deploy it to.

### DIY

If you're familiar with deploying node applications, the built-in Remix app server is production-ready.

Make sure to deploy the output of `remix build`

- `build/`
- `public/build/`

### Using a Template

When you ran `npx create-remix@latest` there were a few choices for hosting. You can run that again to create a new project, then copy over your `app/` folder to the new project that's pre-configured for your target server.

```sh
cd ..
# create a new project, and pick a pre-configured host
npx create-remix@latest
cd my-new-remix-app
# remove the new project's app (not the old one!)
rm -rf app
# copy your app over
cp -R ../my-old-remix-app/app app
```

***

## Original Application

XMA Lab was originally written as a php web application. The source code and binaries of the old application can be downloaded from [bitbucket](https://bitbucket.org/xromm/xmalab/src/master/).

### Download the latest binary release

- Download the latest binary release (1.5.4)
  - [Mac](https://bitbucket.org/xromm/xmalab/downloads/XMALab_1.5.4.dmg)
  - [Windows](https://bitbucket.org/xromm/xmalab/downloads/XMALab_setup-1.5.4.msi)
- User Manual and Version History
  - [XMALab Bitbucket Wiki](https://bitbucket.org/xromm/xmalab/wiki/Home)
- XMALab Tutorial with example data
  - [xmaportal.org/sandbox/](http://xmaportal.org/sandbox/larequest.php?request=explorePublicStudy&StudyID=49&instit=SANDBOX1)

Instructions on how to build the source code can be found [here](https://bitbucket.org/xromm/xmalab/wiki/Instructions%20for%20developers)
