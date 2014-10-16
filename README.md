This is MojoShader with my personal WIP changes related to fully supporting Direct X effect (.fx) file parsing and rendering.

Summary of Changes
----------------
* Misc. fixes to effect and preshader parsing
* Additional effect data parsed
  * Pass state settings
  * Sample state settings
  * Param default values
* Addition of OpenGL effect API that is similiar to the DirectX 9 effect API
  * Shader setup for all techniques+passes
  * Pass render state application
  * Sample state application
* Instance draw support

NOTES
----------------
* These are just the source files I touched
  * If you want to utilize these changes first start with https://hg.icculus.org/icculus/mojoshader/

TODO
----------------
* Properly map Texture params to Sampler params
  * You currently have to set texture units for Sampler param (different then Direct X)
* Basic render state shadowing to minimize redundant state changes (Pass and Sampler state)
* Support all Pass and Sampler state possibilities
* Support assigning default values to all Param types
* Clean up changes and match resident coding style better

About MojoShader
----------------
For more information about MojoShader, visit the website:

http://icculus.org/mojoshader/