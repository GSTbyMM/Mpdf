Note: This is fork of the original extension Mpdf working with mpdf 8.2.5 and MediaWiki 1.43.1.

== Installation ==
1. Download the zip and upload to the extensions dir.
2. Unzip it in the extensions dir.
3. Include the following configurations in the LocalSettings.php file
   wfLoadExtension( 'Mpdf' );

   $wgMpdfToolboxLink = true;
   $wgMpdfTab = true;
   $wgMpdfSimpleOutput = true;
