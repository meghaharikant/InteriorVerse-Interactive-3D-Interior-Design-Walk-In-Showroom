# InteriorVerse – Interactive 3D Interior Design & Walk-In Showroom

InteriorVerse is a Unity-based interior design application that allows users to explore interactive 3D room environments and customize furniture arrangements. It combines a photo-based furniture staging tool with a 3D walk-in showroom for an immersive interior design experience.

## ✨ Features

- **3D Walk-In Showroom:** Explore four different interior environments.
- **Multiple Room Collections:** Living Room, Bedroom, Bathroom, and Kitchen.
- **Furniture Catalog:** Explore sofas, beds, tables, chairs, lamps, rugs, plants, and other furniture.
- **Interactive Navigation:** Walk around the showroom and inspect products.
- **Lighting Modes:** Switch between daylight and warm evening lighting.
- **Furniture Customization:** Drag, rotate, resize, and delete furniture in the photo-based design tool.
- **Design Management:** Save and load interior designs.
- **Undo and Redo:** Reverse or restore design changes.
- **Export Options:** Export furniture design information as CSV.
- **Budget Estimation:** View estimated furniture costs.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Unity 6.5 | 3D application development |
| C# | Application logic and interaction |
| Unity UI | User interface |
| Procedural Generation | Room environments and visual details |
| Unity Lighting | Daylight and evening lighting |
| JSON | Saving and loading designs |
| CSV | Exporting design information |

## 💻 System Requirements

### Software Requirements

- Windows 10 or Windows 11 (recommended)
- Unity Hub
- Unity Editor 6.5 (`6000.5.10f1`)
- Visual Studio or Visual Studio Code (optional, for editing scripts)
- Git (optional, for cloning the repository)

### Hardware Requirements

- Minimum 8 GB RAM (16 GB recommended)
- Dual-core or better processor
- Graphics card supporting DirectX 11 or 12
- At least 5 GB of free storage space (more may be needed during Unity import and development)

## 📥 Installation and Setup

### Step 1: Install Unity Hub

Download and install Unity Hub:

https://unity.com/download

### Step 2: Install Unity Editor

1. Open Unity Hub.
2. Go to **Installs**.
3. Select **Install Editor**.
4. Install Unity 6.5 (`6000.5.10f1`) if available.
5. Include the Windows Build Support module if you want to create a Windows application build.

### Step 3: Clone the Repository

Open a terminal and run:

```bash
git clone https://github.com/YOUR_USERNAME/InteriorVerse.git
```

Alternatively, download the repository as a ZIP file from GitHub and extract it.

### Step 4: Open the Project in Unity

1. Open Unity Hub.
2. Select **Add → Add project from disk**.
3. Browse to the extracted or cloned project folder.
4. Select the folder containing:
   - `Assets`
   - `Packages`
   - `ProjectSettings`
5. Open the project using Unity 6.5.
6. Wait for Unity to import the project and resolve its packages.

## ▶️ How to Run the Application

### Option 1: Run the 3D Walk-In Showroom

1. Open the project in Unity.
2. From the top menu, select:

   **InteriorVerse → Build Unity 6 Walk-in Showroom**

3. Allow Unity to generate the showroom scene.
4. Open the generated scene if it does not open automatically.
5. Click the **Play** button in the Unity Editor.
6. Explore the showroom using the navigation controls.

The showroom includes four room collections:

- Living Room
- Bedroom
- Bathroom
- Kitchen

### Option 2: Run the Photo-Based Interior Designer

1. Open the Unity project.
2. Use the photo-based interior designer setup provided in the project.
3. Import or place a room image using the available room background workflow.
4. Add furniture from the catalog.
5. Arrange and customize furniture using the available controls.
6. Save or export your design.

To use your own room photograph, place the image in:

```text
Assets/InteriorVerse/Background/
```

The supported background workflow uses `room.png` or `room.jpg`.

## 🎮 Showroom Controls

| Control | Action |
|---|---|
| W / Up Arrow | Move Forward |
| S / Down Arrow | Move Backward |
| A / Left Arrow | Move Left |
| D / Right Arrow | Move Right |
| Right Mouse Button + Mouse | Look Around |
| Left Mouse Click | Inspect Product |
| Esc | Release Mouse Control |

## 🪑 Photo Designer Controls

| Action | Function |
|---|---|
| Drag Furniture | Move furniture |
| Select Furniture | Select an item |
| Rotate Left / Right | Change furniture orientation |
| Enlarge / Reduce | Resize furniture |
| Delete | Remove selected furniture |
| Undo / Redo | Reverse or restore changes |
| Save | Save the current design |
| Load | Load a saved design |
| Export CSV | Export furniture information |
| Clear Room | Remove furniture from the design |

## 📁 Project Structure

```text
InteriorVerse/
│
├── Assets/
│   ├── Editor/
│   │   ├── InteriorVerseSetup.cs
│   │   └── InteriorVerseWalkInShowroomSetup.cs
│   │
│   ├── InteriorVerse/
│   │   ├── Background/
│   │   ├── Scripts/
│   │   │   └── PhotoRoomDesigner.cs
│   │   └── WalkInShowroom/
│   │       ├── InteriorVerseWalkInShowroom.cs
│   │       └── ShowroomProduct.cs
│   │
│   └── Resources/
│       └── InteriorVerseUI/
│
├── Packages/
│   └── manifest.json
│
├── ProjectSettings/
│   └── ProjectVersion.txt
│
└── README.md
```

## 💾 Data Storage

The application stores design information locally.

**Saved design (JSON):**

```text
Application.persistentDataPath/InteriorVerse/design.json
```

**Exported design report (CSV):**

```text
Application.persistentDataPath/InteriorVerse/Reports/InteriorVerse-Design.csv
```

The CSV contains furniture and design information. Furniture prices are sample estimates and may not represent actual market prices.

## 🚀 Future Enhancements

- Realistic 3D furniture models and textures.
- Advanced room dimension and measurement tools.
- Real-time furniture placement in 3D.
- AI-powered interior design recommendations.
- Augmented Reality (AR) furniture placement.
- More room styles and furniture collections.
- Improved rendering and realistic shadows.

## ⚠️ Important Notes

- Use the recommended Unity Editor version to avoid compatibility issues.
- The 3D showroom uses procedurally generated environments and materials.
- The photo-based designer overlays furniture images on a room photograph; it does not automatically reconstruct 3D room geometry.
- The application does not automatically provide WebXR or mobile AR functionality.

## 👩‍💻 Project

**Project Name:** InteriorVerse  
**Platform:** Unity  
**Language:** C#  
**Project Type:** Interactive Interior Design Application and 3D Walk-In Showroom

---

**InteriorVerse – Design, Explore, and Experience Your Dream Spaces.**
