["2.3.18", "3.0.20", "3.2.12"].each do |version|
  appraise "rails#{version[0..2]}" do
    gem "activerecord", version
    gem "activesupport", version
    gem "actionpack", version
  end
end
