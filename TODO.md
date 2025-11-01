<<<<<<< HEAD
# TODO: View More / Refresh for Latest News Feature

## Backend Changes
- [x] Update Backend/routes/news.js to support pagination (page, pageSize parameters)
- [x] Add support for fetching new articles since a timestamp (since parameter)
- [x] Return hasMore flag or total count in response

## Frontend Changes
- [x] Modify Frontend/src/pages/Index.tsx to add pagination state (currentPage, hasMore, loadingMore, refreshing)
- [x] Add Refresh button to the UI (e.g., in navbar or above news grid)
- [x] Implement fetchMoreArticles function to load next page and append articles
- [x] Implement refreshArticles function to fetch new articles since last load and prepend them
- [x] Add localStorage caching for articles per category (load on mount if offline)
- [x] Add View More button at bottom of news grid with loading state
- [x] Ensure no duplicate articles when appending or prepending (check URLs)
- [x] Maintain scroll position when appending new articles
- [x] Add toast notification "✨ New stories loaded!" after successful refresh
- [x] Add loading indicators (spinner for View More, shimmer for refresh)
- [x] Handle errors gracefully with toast messages
- [ ] Test and ensure mobile responsiveness

## Testing and Optimization
- [x] Test pagination, refresh, and caching functionality
- [x] Verify no duplicates and proper sorting (newest first)
- [ ] Optimize performance for large lists
=======
# TODO: Remove Avatar from Profile Section

- [x] Remove avatar-related imports (Avatar, AvatarFallback, AvatarImage, Camera)
- [x] Remove avatar-related state variables (avatarFile, avatarPreview)
- [x] Remove handleAvatarChange function
- [x] Update useEffect to not set avatarPreview
- [x] Modify handleSave to not include avatar in form data
- [x] Remove the Avatar Section JSX
>>>>>>> 41b0a99ef6673d708b461b1662677c8318e03b44
