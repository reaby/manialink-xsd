# manialink-xsd
XML schema for manialink v3


## Usage

### Without namespace (old way)

```xml
<?xml version="1.0" encoding="utf-8" standalone="yes"?>
<?xml-model href="https://raw.githubusercontent.com/reaby/manialink-xsd/main/manialink_v3.xsd" ?>

<manialink version="3">
    <-- your manialink content here -->
</manialink>
```

### With namespace

Xml-model directive:

```xml
<?xml version="1.0" encoding="utf-8" standalone="yes"?>
<?xml-model href="https://raw.githubusercontent.com/reaby/manialink-xsd/main/manialink_v3_ns.xsd" ?>

<manialink version="3" xmlns="manialink">
    <-- your manialink content here -->
</manialink>
```

in case the first one doesn't work:

```xml
<?xml version="1.0" encoding="utf-8" standalone="yes"?>
<manialink version="3" xmlns="manialink" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="manialink https://raw.githubusercontent.com/reaby/manialink-xsd/main/manialink_v3_ns.xsd">
 <-- your manialink content here -->
</manialink>
```

