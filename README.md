# TRUStoreApp

An iOS assignment built using **UIKit** and **MVVM**, fetching product data from [FakeStoreAPI](https://fakestoreapi.com/products?limit=7).  
This app demonstrates clean architecture, pagination, layout switching, caching, and more.

---

## 🚀 Features

- ✅ Product list fetched from API
- ✅ Toggle between **grid** and **list** view
- ✅ Pagination (loads 7 products per request)
- ✅ Product detail screen with:
  - Stretchable image header
  - Title, category, price, description
- ✅ Skeleton loading view using `SkeletonView`
- ✅ Offline support via local caching
- ✅ Clean MVVM architecture
- ✅ Fully programmatic UI using `UIKit`
- ✅ Git with atomic commits

---

## 🧱 Architecture

The app follows **MVVM**:
- `Product`: Decodable model
- `APIService`: Handles API requests and caching
- `ProductListViewModel`: Handles pagination and business logic
- `ProductListViewController`: UI, uses ViewModel to render data
- `ProductDetailViewController`: Displays full product details

---

## 📦 Libraries

- [`SDWebImage`](https://github.com/SDWebImage/SDWebImage) – For async image loading
- [`SkeletonView`](https://github.com/Juanpe/SkeletonView) – For elegant loading indicators

---

## 🧪 Future Enhancements

- Add unit tests for ViewModels
- Add UI tests for rendering products
- More advanced caching via `CoreData` or `Realm`
- Search or filter support

---

## 🔧 Setup

1. Clone this repo
2. Open in Xcode
3. Run on any simulator or device

> Minimum deployment target: iOS 13+

---

## 💡 Notes

- No Storyboards used (100% programmatic UI)
- The app works without internet by using cached results
- Layout adapts to screen size
- Uses `UICollectionViewFlowLayout` (no external layout libs)

---

## 📂 Screenshots

| Grid View | List View | Product Detail |
|-----------|-----------|----------------|
| ![grid](screens/grid.png) | ![list](screens/list.png) | ![detail](screens/detail.png) |

---

Made with ❤️ for TRU by Mohamed Elboraey
