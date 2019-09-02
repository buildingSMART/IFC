**Definition
from IAI:** An _IfcTextureVertex_ is a list of 2 (S, T) texture coordinates.

The following additional definitions from ISO/IEC FCD 19775:200x, the Extensible 3D ([X3D](http://www.web3d.org/x3d/specifications/x3d_specification.html){ target="_blank"}) specification, apply:

> Each vertex-based geometry node uses a set of 2D texture coordinates that map textures to vertices. Texture map values ( ImageTexture, PixelTexture) range from [0.0, 1.0] along the S-axis and T-axis. However, texture coordinate values may be in the range (-&infin;,&infin;). Texture coordinates identify a location (and thus a colour value) in the texture map. The horizontal coordinate S is specified first, followed by the vertical coordinate T. If the texture map is repeated in a given direction (S-axis or T-axis), a texture coordinate C (s or t) is mapped into a texture map that has N pixels in the given direction as follows:
> 
>> <pre><b>Texture map location = (C - floor(C)) &times; N<br>			 </b></pre>
> If the texture map is not repeated, the texture coordinates are clamped to the 0.0 to 1.0 range as follows:
> 
>> <pre><b>Texture map location = N,     if C &gt; 1.0,<br>                     = 0.0,   if C &lt; 0.0,<br>                     = C &times; N, if 0.0 &le; C &le; 1.0.</b>
    </pre>
> Texture coordinates may be transformed (scaled, rotated, translated) by supplying a TextureTransform as a component of the texture's definition.
> 


> <font color="#0000ff" size="-1">HISTORY: New entity
in IFC
Release 2x Edition 2.<br>
  </font>