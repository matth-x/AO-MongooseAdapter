# MicroOcppMongoose
Mongoose WebSocket adapter for MicroOCPP

## Dependencies

The following projects must be available on the include path:

- [Mongoose Embedded Networking Library v6.14 / v7.8 / v7.13 - v7.15](https://github.com/cesanta/mongoose/tree/76e6b23a4f0261dd534d33632f42ea1bba99dc85): The MicroOcppMongoose adapter works with the amalgamated files `mongoose.h` and `mongoose.c`. You may need to copy them from the Mongoose-repository into the `src` folder of your project. To configure the Mongoose version in MicroOcppMongoose, set the build flag `MO_MG_USE_VERSION`, e.g. `MO_MG_USE_VERSION=MO_MG_V715`.
- [ArduinoJson v6](https://github.com/bblanchon/ArduinoJson/tree/079ccadbee4100ad0b2d06f11de8c412b95853c1) (no support for v7 yet)
- [MicroOCPP](https://github.com/matth-x/MicroOcpp)

The setup is done if the following include statements work:

```cpp
#include "mongoose.h"
#include <ArduinoJson.h>
#include <MicroOcpp.h>
```

## License

This project is licensed under the GPL as it uses the [Mongoose Embedded Networking Library](https://github.com/cesanta/mongoose). If you have a proprietary license of Mongoose, then the [MIT License](https://github.com/matth-x/MicroOcpp/blob/master/LICENSE) applies.
