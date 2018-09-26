# Texture2D.EncodeToTGA (Unity)

Adds a EncodeToTGA Extension-Method to Texture2D. Uses Run-Length-Encoding and can Encode RGB24 and ARGB32 Formats (equally to EncodeToPNG and EncodeToJPG).

As some software doesn't support RLE-Encoded TGA-Files, also supports uncompressed Encoding. The Default is RLE.

## Usage

```csharp

Texture2D texture;

// Default usage -- write tga-data to file
File.WriteAllBytes("file.tga", texture.EncodeToTGA()); 

// Encode w/o compression -- in most cases you won't need that. 
// Only use, if you work with software that doesn't support Compressed TGAs.
File.WriteAllBytes("file.tga", texture.EncodeToTGA(EncodeToTGAExtension.Compression.None));

```

## (Un)License

This is free and unencumbered software released into the public domain.

Anyone is free to copy, modify, publish, use, compile, sell, or distribute this software, either in source code form or as a compiled binary, for any purpose, commercial or non-commercial, and by any means.

In jurisdictions that recognize copyright laws, the author or authors of this software dedicate any and all copyright interest in the software to the public domain. We make this dedication for the benefit of the public at large and to the detriment of our heirs and successors. We intend this dedication to be an overt act of relinquishment in perpetuity of all present and future rights to this software under copyright law.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

For more information, please refer to <http://unlicense.org/>
