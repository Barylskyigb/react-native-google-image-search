This package is ported from node-google-image-search.
It's using react-native-config instead of dotenv to be usable inside react-native (and is also using es6 instead of old syntax).

Setup

1. Install react-native-config.

2. Create a .env file with your CSE id and api key, for example:
```
CSE_ID=000481220124135128830617:ndojhfef1cq
CSE_API_KEY=AIzaSyBaBZ_fsdfsdfRd36hUSy0PUlqZxfF23sUQ
```

Usage

```
import imageSearch from "react-native-google-image-search";


imageSearch("cats", 0, 5).then(images => {
  return images.map(image => console.log(image.link));
});
```
