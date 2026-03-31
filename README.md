How It Works
PPTX Processing (5-step pipeline):
Scans .rels files — finds all hyperlink relationships pointing to gamma.app
Removes hyperlinks — deletes <Relationship> entries linking to gamma.app
Removes watermark shapes — uses regex to find and remove <p:sp>, <p:pic>, <p:grpSp>, and <mc:AlternateContent> elements containing "Made with Gamma" text or gamma relationship IDs — processes slides, layouts, and masters
Removes branding slide — detects if the last slide is a short Gamma branding slide and removes it (updating presentation.xml, .rels, and [Content_Types].xml)
Cleans metadata — removes Gamma from app.xml and core.xml properties
PDF Processing (4-step pipeline):
Removes annotations — finds and removes link annotations pointing to gamma.app
Content stream cleanup — scans page content streams for "gamma" text blocks (BT...ET) and removes them
Removes last page — removes the Gamma branding page
Cleans metadata — removes Producer/Creator fields referencing Gamma
Key Features:
100% client-side — no server uploads, all processing in-browser
Uses JSZip to unpack/repack PPTX (which is a ZIP archive of XML files)
Uses pdf-lib for PDF manipulation
Depth-aware XML parsing for nested group shapes
Detailed activity log showing exactly what was changed
Drag & drop file upload with visual feedback
