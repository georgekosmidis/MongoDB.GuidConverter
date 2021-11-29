# Base64 Encoding / Decoding GUID bytes

Although this converter was created along with the [MongoDB Shell or Compass query with a GUID](https://blog.georgekosmidis.net/2021/11/29/mongodb-shell-or-compass-query-with-a-guid/) blog post, it is not specifically about MongoDB. On the contrary, it is only about MongoDB if GUIDs are used instead of the native `ObjectId()`.

The problem started because `Base64` converters out there are converting the string representation of a `GUID` to `Base64`, which is not the same as converting the *byte array* of a `GUID` to `Base64`.

It's made with *Blazor WebAssembly* so feel free to play around; your browser is doing all the work not my Azure subscription :)

Here is the link: https://base64guid.azurewebsites.net/

*And if it is a bit slow on startup, just be a bit patient! The Dev/Test tier doesn't have always on!*
