icon_scalable_data = [
  'goa-account-facebook.svg',
  'goa-account-flickr.svg',
  'goa-account-foursquare.svg',
  'goa-account-google.svg',
  'goa-account-mailboxorg.svg',
  'goa-account-msn.svg',
  'goa-account-owncloud.svg',
  'goa-account-pocket.svg',
]

icon_symbolic_data = [
  'goa-account-facebook-symbolic.svg',
  'goa-account-flickr-symbolic.svg',
  'goa-account-foursquare-symbolic.svg',
  'goa-account-google-symbolic.svg',
  'goa-account-mailboxorg-symbolic.svg',
  'goa-account-msn-symbolic.svg',
  'goa-account-owncloud-symbolic.svg',
  'goa-account-pocket-symbolic.svg',
]

icons = [
  ['scalable', icon_scalable_data],
  ['symbolic', icon_symbolic_data],
]

foreach icon: icons
  icon_dir = join_paths(goa_datadir, 'icons', 'hicolor', icon[0], 'apps')

  foreach data: icon[1]
    install_data(
      join_paths(icon[0], data),
      install_dir: icon_dir
    )
  endforeach
endforeach
