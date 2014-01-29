["2.3.18", "3.2.12"].each do |version|
  appraise "rails#{version[0..2]}" do
    if version.start_with?("2")
      gem "mocha", "~> 0.12.0"
    else
      gem "mocha", "~> 0.14.0"
    end
    gem "activerecord", version
    gem "activesupport", version
    gem "actionpack", version
    gem 'mysql2', (version.start_with?("2") ? "~> 0.2.0" : ">= 0.3.0")
  end
end
