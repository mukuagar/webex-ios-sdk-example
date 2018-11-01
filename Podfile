source 'https://github.com/CocoaPods/Specs.git'


use_frameworks!

post_install do |installer|
    installer.pods_project.build_configurations.each do |config|
        config.build_settings.delete('CODE_SIGNING_ALLOWED')
        config.build_settings.delete('CODE_SIGNING_REQUIRED')
    end
end


target 'KitchenSink' do
    platform :ios, '10.0'
    pod 'WebexSDK'
    pod 'Cosmos', '~> 15.0'
    pod 'Toast-Swift', '~> 3.0'
    pod 'FontAwesome.swift','~> 1.3.2'
end


target 'KitchenSinkBroadcastExtension' do
    platform :ios, '11.2'
    pod 'WebexBroadcastExtensionKit'
end
