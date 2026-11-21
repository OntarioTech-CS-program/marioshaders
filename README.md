## Lava Shader


<img width="519" height="302" alt="image" src="https://github.com/user-attachments/assets/8d5dbb1b-3824-4b55-8c86-3ee4d3475a49" />


This lava shader is animated using a scrolling noise texture, which offsets the vertex positions of the each vertex vertically. The way that this shader is different from the water shader from class is that instead of scrolling a sin wave, we're using a noise texture to offset the positions. The chaos of the noise makes the lava look like it's bubbling, and the scrolling of the texture make it look like it's flowing. The noise is also applied as a texture, which makes for a very good lava texture, with different regions looking like they are at different temperatures.


## Fireball Shader

<img width="570" height="247" alt="image" src="https://github.com/user-attachments/assets/12e24c38-4926-4abd-9c96-ab4c96637b98" />

This shader also uses two even faster scrolling noise textures multiplied each other, creating even more chaos. One way that this shader differs from the scrolling texture shaders shown in class is that the noise is also applied to the transparency of the texture, to make the flame more or less transparent in different areas. By making some areas more transparent, it gives the flame a constantly changing shape and outline, just like a real flame. it also makes parts of it semi-transparent, for even more depth and realism. 

## Height Mapping

<img width="691" height="243" alt="image" src="https://github.com/user-attachments/assets/3c6faa70-a2a9-472f-bb0b-18987201d0ce" />


We have added height mapping to add depth to the lighting on the tile texture. The shader that applies the height mapping and textures also uses a tiling/offset node, which allowed us to make the tile pattern repeat a different number of times, and create evenly sized tiles even on our differently scaled terrain pieces. 

<img width="585" height="417" alt="image" src="https://github.com/user-attachments/assets/4a2fb379-9b4a-4880-9c53-736a7ddb01d8" />

There was an unintended consequence of using height mapping, which was that due to how the engine calculates normals from the height map, when you zoom in very close, adjacent UVs can sample the same pixel and create this interesting pyramid effect. Although unintentional, it adds more depth and detail to this texture.

## Complete look

<img width="788" height="495" alt="image" src="https://github.com/user-attachments/assets/1e56dd0d-4a6d-4154-9be7-930df6b2ebbe" />
