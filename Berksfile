source 'https://supermarket.chef.io'

metadata

# load local overrides
berksfile_dir = File.absolute_path(File.join('.', 'lib', 'berksfile'))
Dir.glob(File.join(berksfile_dir, '*.berks')).each do |snippet|
  # rubocop:disable Lint/Eval
  eval File.read(snippet), nil, snippet
end
