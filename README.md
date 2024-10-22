# NewsApp

A news application built with MVVM architecture and Jetpack Compose.

## Major Highlights

- **Jetpack Compose** for modern UI
- **Offline caching** with a **single source of truth**
- **MVVM architecture** for a clean and scalable codebase
- **Dagger Hilt** for efficient dependency injection.
- **Retrofit** for seamless networking
- **Room DB** for local storage of news articles
- **Coroutines** and **Flow** for asynchronous programming
- **Pagination** to efficiently load and display news articles
- **Instant search** for quick access to relevant news
- **Navigation** for smooth transitions between screens
- **WebView** for a seamless reading experience
- **Coil** for efficient image loading
- Pull to refresh for refreshing news content
- Swipe to delete for managing saved news articles

## Features Implemented

- Show top news articles
- Filter news by country, language, and source
- Save news articles for future reference
- Search for specific news articles
- View news articles in a WebView for a detailed reading experience

## Dependency Use

- Jetpack Compose for UI: Modern UI toolkit for building native Android UIs
- Coil for Image Loading: Efficiently loads and caches images
- Retrofit for Networking: A type-safe HTTP client for smooth network requests
- Dagger Hilt for Dependency Injection: Simplifies dependency injection
- Room for Database: A SQLite object mapping library for local data storage
- Paging Compose for Pagination: Simplifies the implementation of paginated lists

## The Complete Project Folder Structure

```
|── NewsApplication.kt
├── common
│   ├── Const.kt
│   ├── NoInternetException.kt
│   ├── dispatcher
│   │   ├── DefaultDispatcherProvider.kt
│   │   └── DispatcherProvider.kt
│   ├── logger
│   │   ├── AppLogger.kt
│   │   └── Logger.kt
│   ├── networkhelper
│   │   ├── NetworkHelper.kt
│   │   └── NetworkHelperImpl.kt
│   └── util
│       ├── EntityUtil.kt
│       ├── NavigationUtil.kt
│       ├── TimeUtil.kt
│       ├── Util.kt
│       └── ValidationUtil.kt
├── data
│   ├── database
│   │   ├── AppDatabaseService.kt
│   │   ├── ArticleDatabase.kt
│   │   ├── DatabaseService.kt
│   │   ├── dao
│   │   │   ├── ArticleDao.kt
│   │   │   └── SavedArticleDao.kt
│   │   └── entity
│   │       ├── Article.kt
│   │       ├── SavedArticleEntity.kt
│   │       ├── SavedSourceEntity.kt
│   │       └── Source.kt
│   ├── model
│   │   ├── ApiArticle.kt
│   │   ├── ApiSource.kt
│   │   ├── Country.kt
│   │   ├── Language.kt
│   │   ├── News.kt
│   │   └── Sources.kt
│   ├── network
│   │   ├── ApiInterface.kt
│   │   └── ApiKeyInterceptor.kt
│   └── repository
│       └── NewsRepository.kt
├── di
│   ├── module
│   │   └── ApplicationModule.kt
│   └── qualifiers.kt
├── ui
│   ├── NewsActivity.kt
│   ├── base
│   │   ├── CommonUI.kt
│   │   ├── NewsDestination.kt
│   │   ├── NewsNavigation.kt
│   │   └── UIState.kt
│   ├── components
│   │   ├── Article.kt
│   │   ├── FilterItem.kt
│   │   ├── FilterItemListLayout.kt
│   │   └── NewsListLayout.kt
│   ├── paging
│   │   └── NewsPagingSource.kt
│   ├── screens
│   │   ├── ArticleScreen.kt
│   │   ├── FilterScreen.kt
│   │   ├── NewsScreen.kt
│   │   ├── SavedScreen.kt
│   │   └── SearchScreen.kt
│   ├── theme
│   │   ├── Color.kt
│   │   ├── Theme.kt
│   │   └── Type.kt
│   └── viewmodels
│       ├── NewsViewModel.kt
│       ├── SearchViewModel.kt
│       ├── SharedViewModel.kt
│       └── filters
│           ├── CountryFilterViewModel.kt
│           ├── LanguageFilterViewModel.kt
│           └── SourceFilterViewModel.kt
└── worker
    └── NewsWorker.kt
```

