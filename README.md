## Community Formulae For API Brew

API Brew is an iOS app to build your own content feed. One of the key features is to build your own cask. This Github repository houses community owned casks that can be imported directly into the App.


## Schema

Top level Fields:
- name: Name of the cask
- image: Any SF Symbol name
- url: URL to use for extracting the data
- pour: One of `pint, mug, snifter`
- extractor: Object containing the extractor logic
   - keys: List of top level fields within the main json to extract information. The result should either be a list of json objects or a single json object at the end.
   - title: The field to use for the title of the view
   - subtitle: The field to use for the subtitle of the view
   - url: The field to use for the url of the view
   - image: The field to use for the image of the view (Only applicable for the pour: mug).

All imports to the repository must follow this format for approvals and eventually being integrated into the brewery.

## Importing

To import simply copy the json and paste it in the app. You can BYOC in `Settings -> Add a new Cask`.

## Contributing

Send over a PR with your favorite cask and I will try to get it merged in soon.