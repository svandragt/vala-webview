# Creating a GTK Native App with Webview

This repo presents a basic approach to building a GTK native app that incorporates a webview component. The objective is to combine a locally served web app with the native app functionality for a seamless user experience.

While launching the web app URL in a browser tab is simpler, it doesn't align with the goal of providing a dedicated native app experience. Some browsers, like Gnome Web, offer the option to install websites as applications, but this requires user interaction and may not be as convenient.

```shell
# Bootstrap
meson build --prefix=/usr && cd build
ninja install

# Build and run
ninja && src/com.github.svandragt.hello-browser --url https://github.com/svandragt/hello-browser
```
![image](https://github.com/svandragt/vala-webview/assets/594871/ad18e3c6-de18-4c74-9965-af2ce1172491)


If you leave out the url parameter it will load example.com.
