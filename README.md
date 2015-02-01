# RecyclerViewElementary
The final idea is to obtain a fully ready RecyclerView (returned programmatically) in one line of code.

A very initial stage of development. There are plans to leave the most basic function for constructing a fully ready RecyclerView while adding different functions returning more customized RecyclerViews (with custom layout managers, different data structures, custom row layouts, etc.)

## How to use
1. Add rve.aar file to your project dependencies.
You may need to use this method to reference an .aar file http://geekgarage.dad3zero.net/local-aar-android-library/
2. Implement `DataModel` interface to describe your data structure.
3. Build your RecyclerView:

    ```java
    List<DataModel> data = getData(); //your data
    RecyclerView view = new RecyclerViewBuilder(this).setData(data).build();
    ```

4. Add RecyclerView to your layout.

You can find an example of usage in the `sample` module.

## Coming soon
- [x] basic construction of purely textual RecyclerViews
- [x] setting a custom LayoutManager
- [x] setting an onClickListener
- [x] setting a custom layout from layout resources (implemented for textual RecyclerViews)
- [ ] support for images in data structures
- [ ] other customizations (some are already implemented: margins, padding, corner radii, etc.)