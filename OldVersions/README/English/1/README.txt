
***

# WarmWelcome

`🌐️👋️🌐️💾️ WarmWelcome is a protocol for opening a single web-page upon connecting to a Wi-Fi network/hotspot (warm spot) which gives you basic information about the network.`

## Summary

A protocol for opening a single web-page upon connecting to a Wi-Fi network/hotspot (warm spot) which gives you basic information about the network (with a 2,097,152 byte (2.00 MiB) text limit, and a 4 gigabyte media limit)

## Is this a captive portal?

Kind of. It isn't a captive requirement, as users aren't required to accept anything to access the network through WarmWelcome, but it is something that will pop up first thing when a network is reached (unless the user chooses to disable warm greetings via settings)

## WarmGreeting vs WarmWelcome

WarmGreeting is the name of the implementation, while WarmWelcome is the name of the protocol.

## Media files and limitations

There is a 2 MiB (2,097,152 byte) limit for text that can be placed on a WarmWelcome page, and a 4 gigabyte media limit (users who have their connection set to metered will be asked before any media is loaded, and connections below 200 Megabits will receive a 1 gigabyte media limit, 100 megabits connections will receive a 500 megabyte media limit, and connections below this threshold will receive a 4 megabyte media limit)

Supported media formats include:

- PNG
- JPG
- SVG
- GIF
- MP4
- MP3
- OGG/OGA
- WebM/NetV

WebP is planned to not be supported, as it is a restrictive, inefficient, and poorly supported format. However, I have made the exception of including WebM, as it is not restrictive, efficient, widely supported, and is already a recognizable standard.

## Implementation

For users who choose to disable JavaScript, there will be separate implementations written in other web languages, but the softwares main implementation language is Python (which can be used to generate the necessary source code for the software, if it isn't included separately)

## Integration

If this becomes a standard, developers will need to integrate support for the protocol into their operating systems to become compliant. Compliance requires the following 3 conditions:

- [ ] A setting to enable/disable WarmWelcome
- [ ] Proper media support for the specified formats, and no other formats outside of the specification
- [ ] No malicious functions within the implementation (such as telling users they cannot exit WarmWelcome)

***

# File info

**File version:** `1 (2023, Monday, June 5th at 10:55 pm PST)`

***
