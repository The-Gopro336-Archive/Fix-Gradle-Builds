# PSA: Fixing gradle builds post 1/29/21
After around the 29-30th of January spongepowered, the maker of mixins used in minecraft forge clients and mods made some changes to their side that breaks building of all forge mods. Fortunately it is only a minor change an can be fixed in seconds.

This is the error you get if you try to compile a forge mod right now:
![Pic](https://media.discordapp.net/attachments/712745558673981510/806005063180353596/Error.png?width=2520&height=476)


The problem lies in your build.gradle file, The server has switched from a http protocol to a https protocol, so in your build.gradle file change all of the urls that have the word SPONGE in them. DON'T change any of the other urls. (There are normally 2 urls)

![Pic](https://media.discordapp.net/attachments/712745558673981510/806005076602257408/url.png)
![Pic](https://media.discordapp.net/attachments/712745558673981510/806005089751924756/url2.png)

Change http://repo.spongepowered.org/maven
to https://repo.spongepowered.org/repository/maven-public/


or do it the chad way


Change http://repo.spongepowered.org/maven
to https://repo.spongepowered.org/maven

Hope this helps!

Star and share!

