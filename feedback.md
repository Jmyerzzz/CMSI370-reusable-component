

## Jackson Myers

##### https://github.com/lmu-cmsi370-fall2017/reusable-component-Jmyerzzz.git

| | Feedback | Points | Notes |
| --- | --- | ---: | --- |
| **Direct manipulation implementation (_2b_, _3a_, _3b_, _4a_, _4b_, _4d_)** | Works pretty well; no glitches seen. | 20 |  |
| **Notification mechanism (callback/event) (_2b_, _3b_, _4a_, _4b_, _4d_)** | Notifier includes `$current` as `this`, then `percentage`. | 20 |  |
| **Plugin model implementation (_2b_, _3b_, _4a_, _4b_, _4d_)** | `data(‘percent’)` works well for the model. | 20 |  |
| **Web front end integration (_2b_, _3a_, _3b_, _4a_, _4b_, _4d_)** | Integration was not successful…because of file order. Remember that JavaScript executes code in the order that it encounters `script` elements in the browser. The `slider` plugin does not seem to exist because as submitted, the web front end was loading _slider.js_ **after** loading and initializing the `AccuWeatherReport` controller. Thus, at that point, `slider` did not yet exist.<br><br>Moving the _slider.js_ `script` element to _before_ the _accuweather.js_ element solves the problem. Unfortunately, because you ran into this, actual integration code was not written. The trial code would have needed to go inside the `AccuWeatherReport` object in order to access and control the city presets. | 12 | Unsuccessful integration due to incorrect JavaScript file loading order |
| **Inappropriate third-party library use** | No third-party contraband found. |  |  |
| **Test Suite (_4a_, _4b_, _4d_)** | 3 out of 3—That’s pretty low for this plugin. A look at these three tests reveals a few untested cases. One significant one: what if the user sets up the plugin without any options? (i.e., `$(selector).slider()`) There are a few other situations that are untested.<br><br>**Statements** 21/24 (87.50%)<br>**Branches** 4/8 (50.00%)<br>**Functions** 1/1 (100.00%)<br>**Lines** 21/24 (87.50%) | 16 | A few easy-to-reach cases—just need the right simulated events inside the right unit tests
| **Code Style (_4c_)** | No errors. |  |  |
| **Version Control (_4e_)** | 8 commits |  |  |
| **Punctuality (_4f_)** | on time |  |  |
|  |  | **88** | **Total** |
