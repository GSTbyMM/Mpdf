Note: This is fork of the original extension Mpdf working with mpdf 8.2.5 and MediaWiki 1.43.1.

== Installation ==
1. Download the zip and upload to the extensions dir.
2. Unzip it in the extensions dir.
3. Include the following configurations in the LocalSettings.php file <br>

   wfLoadExtension( 'Mpdf' );<br>
    <br>
   $wgMpdfToolboxLink = true;<br>
   $wgMpdfTab = true;<br>
   $wgMpdfSimpleOutput = true;<br>

== Configuration ==

The following optional parameters can be added to LocalSettings.php:

=== Font Configuration ===

Use these settings to enable support for different languages, including RTL languages like Farsi, Arabic, and Hebrew.

; $wgMpdfDefaultFont
: Sets the default font for PDF generation. Supports fonts with Unicode characters.
: Default: 'DejaVuSans' (supports Farsi, Arabic, Chinese, etc.)
: Example: <code>$wgMpdfDefaultFont = 'DejaVuSans';</code>
: Other options: 'DejaVuSerif', 'Liberation Sans', 'FreeSerif', 'Noto Sans'

; $wgMpdfAutoScriptToLang
: Automatically detects text script and applies appropriate font features for proper character shaping (essential for Arabic/Farsi rendering).
: Default: true
: Example: <code>$wgMpdfAutoScriptToLang = true;</code>

; $wgMpdfUseAdobeCJK
: Enables Adobe CJK font support for better Chinese, Japanese, Korean character rendering.
: Default: false
: Example: <code>$wgMpdfUseAdobeCJK = false;</code>
