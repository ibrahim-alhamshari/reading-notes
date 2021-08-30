## Create dynamic lists with RecyclerView

- **RecyclerView** is the ViewGroup that contains the views corresponding to your data. Each individual element in the list is defined by a *view holder* object. 

- When we creating the view holder, there is no data associated with it yet. So, the `RecyclerView` binds the data to that view holder.

- **LayoutManager** class: It is responsible for measuring and positioning item views within a RecyclerView as well as determining the policy for when to recycle item views that are no longer visible to the user. 

### Implementing the adapter and view holder

- The **ViewHolder** is a wrapper around a View that contains the layout for an individual item in the list.
- The **Adapter** creates ViewHolder objects as needed, and also sets the data for those views.
- The **Adapter** and the **ViewHolder** control the by the display of the data.

- **To implement the adapter you need to implement(override) three methods:**
1. `onCreateViewHolder()`: *RecyclerView* calls this method whenever it needs to create a new ViewHolder. 
2. `onBindViewHolder()`: *RecyclerView* calls this method to associate a ViewHolder with data. The method fetches the appropriate data and uses the data to fill in the view holder's layout. 
3. `getItemCount()`: RecyclerView calls this method to get the size of the data set.

### Resources
- https://developer.android.com/guide/topics/ui/layout/recyclerview#java