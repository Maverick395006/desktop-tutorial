gradle/plugins{

id 'kotlin-android-extensions'

}

  .................................................
 ////////// Volley Dependency ////////////////////
'''''''''''''''''''''''''''''''''''''''''''''''''
implementation("com.android.volley:volley:1.2.0")








  .................................................
 ////////// Annotation Processing ////////////////
'''''''''''''''''''''''''''''''''''''''''''''''''

plugins {
    id 'kotlin-kapt'
}


  ............................................
 ////////// For Data Binding ////////////////
''''''''''''''''''''''''''''''''''''''''''''

buildFeatures{
        dataBinding = true
    }


  .................................................
 ////////// Life Cycle Dependency ////////////////
'''''''''''''''''''''''''''''''''''''''''''''''''

	def lifecycle_version = "2.4.0-alpha03"
        // ViewModel
        implementation "androidx.lifecycle:lifecycle-viewmodel-ktx:$lifecycle_version"
        // LiveData
        implementation "androidx.lifecycle:lifecycle-livedata-ktx:$lifecycle_version"


  .................................................
 ////////// Coroutines Dependency ////////////////
'''''''''''''''''''''''''''''''''''''''''''''''''
	
	// Core Implemetation
	implementation 'org.jetbrains.kotlinx:kotlinx-coroutines-core:1.5.2'
	// Android specific coroutines Library
	implementation 'org.jetbrains.kotlinx:kotlinx-coroutines-android:1.5.2'



  ...............................................
 ////////// Retrofit Dependency ////////////////
'''''''''''''''''''''''''''''''''''''''''''''''

    implementation 'com.squareup.retrofit2:retrofit:2.9.0'
    implementation 'com.squareup.retrofit2:converter-gson:2.9.0'



  ...........................................
 ////////// Room Dependency ////////////////
'''''''''''''''''''''''''''''''''''''''''''
    def room_version = "2.3.0"
    implementation "androidx.room:room-runtime:$room_version"
    kapt "androidx.room:room-compiler:$room_version"
    implementation "androidx.room:room-ktx:$room_version"
