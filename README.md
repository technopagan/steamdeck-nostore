# steamdeck-nostore
CSS Loader Plugin (see Decky Loader => CSS Loader) to hide the "Store" button on SteamDeck's main menu.

## Word of Warning
Since this simple plugin just hides the Store button via CSS, it does not remove the elememt from the DOM, which means that there will be an invisible navigation step between "Library" and "Friends". Controller navigation behaves the same as keyboard navigation (e.g. tabbing through menus) and there is nothing CSS can do about it in this case.

The proper solution would be to remove the entire node (all the nested divs for the "Store" menu item) from the DOM, but that would require a standalone Decky Loader plugin and working with React to perform the DOM manipulation. Yuck.

For me personally, hiding the "Store" button like this with CSS only probably does the trick of stopping my inner instant gratification monkey in its tracks. So my motivation of building the "proper" solution is not high at the moment. Let's see how long until the invisible navigation step glitch annoyes me enough to fix it.