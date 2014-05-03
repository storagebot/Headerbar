# Header for firefox-extension-htitle

Here is complete tutorial of Firefox GNOME integration

1. Install all software from this list(don't restart after installing each one):
 * [GNOME 3 theme for Firefox](https://addons.mozilla.org/firefox/addon/adwaita/), or if you can't wait for 3.12-style tabs - use [beta](https://github.com/gnome-integration-team/firefox-gnome/issues/241)
 * [GNOME 3 Theme Tweak extension](https://addons.mozilla.org/firefox/addon/gnome-theme-tweak/)
 * [Hide Tab Bar With One Tab](https://addons.mozilla.org/en-US/firefox/addon/hide-tab-bar-with-one-tab/)
 * [HTitle](https://addons.mozilla.org/firefox/addon/htitle/) - for hiding titlebar
 * [GNotifier](https://addons.mozilla.org/firefox/addon/gnotifier/) - for native notifications
 * [Stylish](https://addons.mozilla.org/firefox/addon/stylish/) - for adjusting userstyles

2. Restart your browser, go to [Addons](about:addons), find GNOME Theme Tweak options and enable options you like, find HTitle options and select hide titlebar "Always" option

3. Go to Styles section and add userstyle:

        @-moz-document url(chrome://browser/content/browser.xul) {
    
            #nav-bar {
                background-image: -moz-linear-gradient(rgba(255, 255, 255, 1), rgba(255, 255, 255, 0)) !important;
            }
    
            /* Bigger paddings for better dragging experience */
        
            #navigator-toolbox:not([tabsontop="true"]) #nav-bar {
                padding: 3px 3px 6px 3px !important;
            }
        
            #urlbar {
                margin: 0 36px !important;
            }
        }

4. Press "Download ZIP" on the right of this page, copy "Headerbar-master" folder from downloaded archive into <code>~/.local/share/themes/</code> - if this folder does not exist - create it

5. Switch window theme to "Headerbar-master" using GNOME Tweak Tool
