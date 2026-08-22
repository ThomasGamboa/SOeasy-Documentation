# **SOeasy — Lightweight ScriptableObject Manager**

One window for every ScriptableObject in your project — auto-organized by folder, searchable, and editable without ever leaving it.

---

## **Getting Started**

1. Open the window from **Tools > VoxelNest > SOeasy**.
2. Expand **Scan Folders** and add one or more folders — or enable **Scan Full Project** to scan everything at once.
3. Your ScriptableObjects appear grouped by folder automatically. Click one to edit it.

No configuration, no registering types, no setup asset. Point it at a folder and it works.

---

## **Browsing**

- Nested folders show as collapsible groups — click the header or the arrow to expand/collapse.
- **Search** (toolbar) filters live by name.
- **Sort** (toolbar) toggles between alphabetical and last-modified.
- Drag a group's "⠿" handle to reorder it among its siblings — the order is saved automatically.
- Each group's **⋮** menu has **Rename**, which only changes its display label in SOeasy, not the folder itself.

## **Editing**

- Click any ScriptableObject to open it in a floating inspector next to your selection.
- Arrow keys move the selection between groups and items; Enter selects and pings the asset in the Project window.
- Escape closes the floating inspector.
- Editing uses Unity's standard Inspector underneath, so field changes support Ctrl+Z like anywhere else in Unity.

## **Creating, Renaming, Deleting**

- Every group's **⋮** menu lists every ScriptableObject-derived class in your project, organized by inheritance — creating a new one is one click, and you can name it immediately.
- Right-click any item for **Rename**, **Delete**, or **Select in Project**.
- Creating an asset is undoable with Ctrl+Z. Deleting moves it to your OS trash rather than deleting it permanently — it can be recovered from there if needed.

## **Multi-Select & Bulk Actions**

- **Shift+click** selects a range; **Ctrl/Cmd+click** adds or removes individual items.
- Right-click a multi-selection for **bulk Delete** or **bulk Rename** (renames sequentially: `Name_0`, `Name_1`, `Name_2`...).

---

## **Pro Features**

### Pin
Pin any ScriptableObject from its right-click menu. Pinned items always appear in a **Pinned** group at the very top of the list — regardless of which folders are currently scanned or which workspace is active. Bulk-select and right-click to Pin/Unpin several at once.

### Colors
Give any group a custom color, picked from Unity's own native color picker (group **⋮** menu → **Set Color...**). Selecting or expanding a colored group automatically uses a brighter or darker variant of that same color — no extra configuration needed.

### Icons
Assign a custom icon to any group from a folder of plain PNGs (default: `Assets/VoxelNest/SOeasy/Modules/Icons/images`, or point elsewhere via **Tools > VoxelNest > SOeasy > Set Icon Folder...**). Regular textures work directly — no need to reimport them as sprites or touch their alpha settings.

### Workspaces
Named, exclusive folder sets — useful for focusing on one system (e.g. "Combat" or "Economy") without the rest of your project's ScriptableObjects cluttering the view. Switch between workspaces (or back to "All") from the toolbar button. Add a scanned folder to a workspace directly from its row under Scan Folders.

### Find References
Right-click any ScriptableObject → **Find References** to see every asset that points to it — prefabs, scenes, materials, other ScriptableObjects. Backed by a cached reverse-dependency index built off the main thread, so it stays fast even in large projects: the first search in a session builds the index once, every search after that is instant, and it updates itself automatically as your project changes.

---

## **Free vs. Pro**

| | Free | Pro |
|---|:---:|:---:|
| Scan, browse, search, sort | ✓ | ✓ |
| Create / rename / delete | ✓ | ✓ |
| Multi-select & bulk actions | ✓ | ✓ |
| Drag-to-reorder groups | ✓ | ✓ |
| Pin | | ✓ |
| Group colors | | ✓ |
| Group icons | | ✓ |
| Workspaces | | ✓ |
| Find References | | ✓ |
