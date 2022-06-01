# Recycler View

#### The RecyclerView is a ViewGroup that renders any adapter-based view in a similar way. It is supposed to be the successor of ListView and GridView. One of the reasons is that RecyclerView has a more extensible framework, especially since it provides the ability to implement both horizontal and vertical layouts. Use the RecyclerView widget when you have data collections whose elements change at runtime based on user action or network events.

### If you want to use a RecyclerView, you will need to work with the following:

- RecyclerView.Adapter - To handle the data collection and bind it to the view
- LayoutManager - Helps in positioning the items
- ItemAnimator - Helps with animating the items for common operations such as Addition or Removal of item

![RecyclerView](https://user-images.githubusercontent.com/97638932/165623874-68adf76b-497a-4d39-b963-742b878b99e9.png)

#### Furthermore, it provides animation support for RecyclerView items whenever they are added or removed, which had been extremely difficult to do with ListView. RecyclerView also begins to enforce the ViewHolder pattern too, which was already a recommended practice but now deeply integrated with this new framework.

