dataconf = configuration_data()
dataconf.set('BACKGROUNDDIR', backgrounddir)
dataconf.set('datadir', datadir)

backgrounds = [
  'adwaita-d.svg',
  'adwaita-l.svg',
  'amber-d.jxl',
  'amber-l.jxl',
  'blobs-d.svg',
  'blobs-l.svg',
  'drool-d.svg',
  'drool-l.svg',
  'fold-d.jxl',
  'fold-l.jxl',
  'geometrics-d.jxl',
  'geometrics-l.jxl',
  'glass-chip-d.jxl',
  'glass-chip-l.jxl',
  'lcd-rainbow-d.jxl',
  'lcd-rainbow-l.jxl',
  'map-d.svg',
  'map-l.svg',  
  'sheet-d.jxl',
  'sheet-l.jxl',
  '1.jpg',
  '2.jpg',
  '3.jpg',
  '4.jpg', 
  '5.jpg',
  '6.jpg',
  '7.png',
  '8.png',
  '9.jpg',
  '10.jpg', 
  '11.jpg',
  '12.jpg', 
  '13.png',
  '14.png',
  '15.png',
  '16.png', 
  '17.jpg',
  '18.jpg',   
]

install_data(backgrounds, install_dir: backgrounddir)

foreach metadata : [
  'adwaita.xml',
  'amber.xml',
  'blobs.xml',
  'drool.xml',
  'fold.xml',
  'geometrics.xml',
  'glass-chip.xml',
  'lcd-rainbow.xml',
  'map.xml',  
  'sheet.xml',
  '1.xml',
  '2.xml',
  '3.xml',
  '4.xml',
  '5.xml',
  '6.xml',
  '7.xml',
  '8.xml',
  '9.xml']
  configure_file(
    input: metadata + '.in',
    output: metadata,
    configuration: dataconf,
    install: true,
    install_dir: metadatadir
  )
endforeach
