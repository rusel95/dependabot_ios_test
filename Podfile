platform :ios, '14.0'
inhibit_all_warnings!

target 'Test' do

    pod 'RestKit', '0.27.3'
    pod 'AFNetworking', '4.0.1' # DEPRECATED -> need to be removed in favour of Alamofire/URLSession
    pod 'AsyncImageView', '1.6' # DEPRECATED -> need to be removed in favour of AlamofireImage
    pod 'SVPullToRefresh', '0.4.1'
    pod 'SVProgressHUD', '2.2.5', :modular_headers => true
    pod 'Dropbox-iOS-Dropins-SDK', '1.2.1'
    pod 'AWSCore', '2.19.1'
    pod 'AWSS3', '2.19.1'
    pod 'AWSCognito', '2.19.1'
    pod 'MGSwipeTableCell', '1.6.14'
    pod 'HPGrowingTextView', '1.1'
    pod 'FBNotifications', '1.0.1'
    pod 'AppAuth', '1.6'
    pod 'GoogleAPIClientForREST/Drive', '3.0.0'
    pod 'GTMAppAuth', '2.0.0'
    pod 'Firebase', '10.5.0'
    pod 'FirebaseCore', '10.5.0', :modular_headers => true
    pod 'FirebaseDatabase', '10.6.0'
    pod 'FirebaseAuth', '10.5.0', :modular_headers => true
    pod 'FirebaseAnalytics', '10.5.0'
    pod 'FirebaseRemoteConfig', '10.5.0', :modular_headers => true
    pod 'FirebaseMessaging', '10.5.0'
    pod 'FirebaseCrashlytics', '10.5.0'
    pod 'FirebaseInstallations', '10.5.0'
    pod 'GoogleUtilities', '7.11.0', :modular_headers => true
    pod 'AppsFlyerFramework', '6.9.2' # DEPRECATED
    pod 'Alamofire', '~> 4.9.0' # Need a number of refactoring to update to latest version
    pod 'AlamofireImage', '~> 3.6.0'
    pod 'ObjectMapper', '4.2.0'
    pod 'Bond', '7.8.1' # Have to removed in favour of Combine
    pod 'SwiftLint', '0.50.3'
    pod 'JTAppleCalendar', '8.0.4'
    pod 'MaterialComponents/Chips', '124.2.0', :modular_headers => true
    pod 'TikTokOpenSDK', '~> 5.0.14'

end

post_install do |installer|
    installer.pods_project.targets.each do |target|
        puts "#{target.name}"
        target.build_configurations.each do |config|
          config.build_settings.delete 'IPHONEOS_DEPLOYMENT_TARGET'
        end
    end
end
