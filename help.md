# JT Magic Revolve - User Guide

**Version:** 1.0.0  
**Compatible with:** Autodesk Fusion 360  
**Developer:** Giovanni Tommasi - JT Plugin Development

---

## 📋 Overview

JT Magic Revolve is a powerful plugin for Autodesk Fusion 360 that enables you to create multiple copies of 3D bodies with controlled translation and rotation along separate axes. Perfect for creating complex patterns, spirals, and repetitive structures where you need to generate multiple instances of objects with precise positioning and rotation control.

The plugin is available in two versions:
- **Trial Version:** Basic revolving with limitations
- **Pro Version:** Full-featured revolving with advanced capabilities

---

## 🚀 Quick Start Guide

### Step 1: Access the Plugin
1. Open Autodesk Fusion 360
2. Navigate to the **SOLID** workspace
3. In the **CREATE** panel, locate the **JT Magic Revolve** button
4. Click the button to launch the revolving dialog

### Step 2: Select Your 3D Body
1. In the dialog, click the **Body to Duplicate** field
2. Select the 3D body you want to revolve from your design
3. The plugin will automatically analyze the body properties

### Step 3: Configure Translation Axis
1. **Translation Axis:** Choose the axis for body movement (REQUIRED):
   - **TRIAL Version:** Only construction axes (X, Y, Z)
   - **PRO Version:** Linear edges, sketch lines, construction axes

### Step 4: Configure Rotation Axis (Optional)
1. **Rotation Axis:** Choose the axis for body rotation (OPTIONAL):
   - **TRIAL Version:** Only construction axes (X, Y, Z)
   - **PRO Version:** Linear edges, sketch lines, construction axes
   - If not selected, will use the translation axis

### Step 5: Set Operation Parameters
1. **Operation Priority:** Choose the order of operations:
   - **Rotation:** Rotate first, then translate (classic spirals)
   - **Translation:** Translate first, then rotate (distributed patterns)
2. **Translation Distance:** Enter the spacing between bodies (in current units)
3. **Number of Pieces:** Specify how many bodies to create
4. **Rotation Angle:** Set the rotation increment between bodies
5. **Name Root:** Customize the naming pattern for created bodies

### Step 6: Execute Revolving
1. Review the preview of the operation
2. Click **OK** to execute the revolving
3. The plugin will create individual bodies with specified positioning and rotation
4. Pro version automatically organizes bodies in timeline groups

---

## 🆓 Trial Version Features

The trial version provides essential revolving capabilities:

### ✅ Included Features:
- **Basic Revolving:** Up to 2 bodies per operation
- **Construction Axes Only:** X, Y, Z axes for translation and rotation
- **Operation Priority:** Choose between Rotation→Translation or Translation→Rotation
- **Automatic Naming:** Standard naming convention
- **Body Analysis:** Dimension validation and warnings

### ⚠️ Limitations:
- Maximum 2 bodies per operation
- Only construction axes (X, Y, Z) supported
- No timeline grouping
- Final success dialog box shown

### 💡 Trial Version Workflow:
1. Select body to revolve
2. Choose translation axis (construction axes only)
3. Optionally choose rotation axis (construction axes only)
4. Set operation priority, distance, number of pieces, and rotation angle
5. Plugin creates revolved bodies with standard names

---

## 🚀 Pro Version Features

The Pro version unlocks the full potential of body revolving:

### ✅ Advanced Features:
- **Unlimited Revolving:** Up to 1000 bodies per operation
- **All Axis Types:** Linear edges, sketch lines, construction axes
- **Timeline Grouping:** Organizes bodies in timeline folders
- **Custom Naming:** Personalized naming patterns
- **Priority Support:** Direct email support
- **No Final Dialog:** Clean workflow without interruption

### 🎯 Pro Version Workflow:
1. Select body to revolve
2. Choose any translation axis (all types supported)
3. Optionally choose any rotation axis (all types supported)
4. Set custom parameters and naming
5. Execute unlimited revolving operations
6. Automatic timeline organization
7. Professional naming conventions

---

## 📐 Detailed Usage Instructions

### Body Selection
- **Supported Types:** Solid bodies, surface bodies
- **Requirements:** Body must be a single, continuous object
- **Size Limits:** No specific size limitations
- **Validation:** Plugin checks for valid geometry automatically

### Translation Axis Configuration
- **TRIAL Version:** Only construction axes (X, Y, Z of origin)
- **PRO Version:** Linear edges, sketch lines, construction axes
- **Purpose:** Defines the direction of body movement
- **Visual Preview:** Shows axis direction in dialog

### Rotation Axis Configuration
- **TRIAL Version:** Only construction axes (X, Y, Z of origin)
- **PRO Version:** Linear edges, sketch lines, construction axes
- **Purpose:** Defines the axis around which bodies rotate
- **Optional:** If not selected, uses translation axis
- **Visual Preview:** Shows axis direction in dialog

### Operation Priority Configuration
- **Rotation→Translation:** Rotate first, then translate
  - Best for: Classic spiral patterns
  - Effect: Bodies rotate around their original position, then move
- **Translation→Rotation:** Translate first, then rotate
  - Best for: Distributed patterns
  - Effect: Bodies move to new position, then rotate around that position

### Distance Configuration
- **Positive Values:** Move in positive direction along axis
- **Negative Values:** Move in negative direction along axis
- **Zero Distance:** Bodies remain at same position (rotation only)
- **Units:** Uses current Fusion 360 document units
- **Smart Calculation:** Plugin validates reasonable distances

### Number of Pieces Configuration
- **Trial Version:** Maximum 2 pieces
- **Pro Version:** Maximum 1000 pieces
- **Minimum:** 1 piece (original body only)
- **Validation:** Plugin warns for excessive body counts

### Rotation Angle Configuration
- **Positive Values:** Clockwise rotation
- **Negative Values:** Counter-clockwise rotation
- **Zero Angle:** No rotation between bodies
- **Range:** -360° to +360° per body
- **Cumulative:** Each body rotates relative to the previous

### Naming Conventions
**Trial Version:**
- Format: `[NameRoot]_001`, `[NameRoot]_002`, etc.
- Automatic numbering with zero-padding
- Default root: "Revol"

**Pro Version:**
- **Custom Root:** Choose your own naming pattern
- **Smart Numbering:** Automatic sequential numbering
- **Pattern Examples:**
  - `Spiral_Part_001`, `Spiral_Part_002`
  - `Pattern_A_001`, `Pattern_A_002`
  - `Custom_Name_001`, `Custom_Name_002`

---

## 🔧 Advanced Features (Pro Only)

### Timeline Organization
The Pro version automatically creates organized timeline groups:
- **Group Name:** Based on original body name and operation
- **Chronological Order:** Bodies organized sequentially
- **Easy Management:** Expand/collapse groups for clean timeline

### Pattern Creation Strategies

**Spiral Patterns - Best For:**
- Decorative elements and ornaments
- Artistic installations
- Engineering components like springs
- Architectural features
- **Setup:** Rotation priority, same axis for both operations

**Linear Arrays - Best For:**
- Assembly line patterns
- Manufacturing fixtures
- Educational demonstrations
- Prototype development
- **Setup:** Translation priority, zero rotation angle

**Circular Patterns - Best For:**
- Gear assemblies
- Decorative rings
- Mechanical components
- Artistic sculptures
- **Setup:** Zero translation distance, any rotation angle

**Complex Patterns - Best For:**
- Artistic installations
- Advanced engineering components
- Custom decorative elements
- **Setup:** Separate axes, different priorities, creative angle/distance combinations

### Parameter Optimization Tips
- **Spiral Creation:** Combine distance with rotation for spiral effects
- **Linear Arrays:** Use zero rotation for straight lines
- **Circular Patterns:** Use zero distance with rotation
- **Complex Patterns:** Experiment with different angle/distance combinations
- **Parallel Axes:** Similar to traditional spiral behavior
- **Perpendicular Axes:** Creative patterns and arrangements

---

## ⚙️ Technical Specifications

### System Requirements
- **Software:** Autodesk Fusion 360 (Version 2.0.18000 or later)
- **Operating System:** Windows 10/11, macOS 10.15+
- **Memory:** Minimum 8GB RAM recommended
- **Storage:** 50MB trial space for plugin files

### Performance Guidelines
- **Optimal Body Count:** 10-200 bodies for best performance
- **Large Bodies:** Bodies over 50cm may require longer processing
- **Complex Geometry:** Curved surfaces may increase processing time
- **Memory Usage:** Large body counts consume more system memory

### File Format Support
- **Input:** Native Fusion bodies (solid and surface)
- **Output:** Individual Fusion bodies in current document
- **Export:** Compatible with all Fusion export formats
- **Integration:** Works with existing Fusion workflows

---

## 🛠️ Troubleshooting

### Common Issues and Solutions

**"Body selection is invalid"**
- Ensure you've selected a valid solid or surface body
- Check that body is not part of a component assembly
- Verify body has proper geometry

**"Translation axis is invalid"**
- **TRIAL:** Ensure selected axis is a construction axis (X, Y, Z)
- **PRO:** Ensure selected edge is linear, sketch line is valid, or construction axis exists
- Verify axis has proper direction and length

**"Rotation axis is invalid"**
- **TRIAL:** Ensure selected axis is a construction axis (X, Y, Z)
- **PRO:** Ensure selected edge is linear, sketch line is valid, or construction axis exists
- Verify axis has proper direction and length

**"Too many bodies requested"**
- **Trial version:** Reduce body count to 2 or upgrade to Pro
- **Pro version:** Confirm intention for large body count
- Consider performance impact of large operations

**"Revolving operation failed"**
- Check body geometry for errors
- Ensure adequate system memory
- Try simpler geometry or fewer bodies
- Verify axis selections are valid

**Help not working**
- Ensure internet connection is active
- Check firewall settings for browser access
- Try refreshing the help page

### Performance Optimization
- **Close unnecessary applications** before large revolving operations
- **Save your work** before running complex patterns
- **Use Preview mode** to verify settings before execution
- **Consider batch processing** for multiple bodies

---

## 📞 Support and Contact

### Trial Version Support
- **Documentation:** This help page and GitHub repository
- **Community:** GitHub Issues and discussions
- **Updates:** Automatic through Autodesk App Store

### Pro Version Support
- **Email:** jtplugin@ajl.vision
- **Feature Requests:** Priority consideration for new features

### Additional Resources
- **GitHub Repository:** https://github.com/jtplugin/fusion-magic-revolve
- **Privacy Policy:** https://jtplugin.github.io/privacy-policy
- **Terms of Service:** https://jtplugin.github.io/fusion-magic-revolve/terms_of_service
- **Company Website:** https://github.com/jtplugin

---

## 🔄 Version History

### Version 1.0.0 (Current)
- Initial release with Trial and Pro versions
- Separate translation and rotation axes
- Operation priority control (Rotation→Translation vs Translation→Rotation)
- Timeline organization (Pro)
- Custom naming patterns (Pro)
- Comprehensive validation system
- F1 Help integration

### Planned Features
- Custom path following

---

## 📜 Legal Information

**Copyright © 2025 Giovanni Tommasi - JT Plugin Development**

This software is distributed through the Autodesk App Store under the terms specified in our Terms of Service. By using this plugin, you agree to our Privacy Policy and Terms of Service.

**Privacy:** We respect your privacy. This plugin does not collect or transmit your design data. License verification only transmits machine ID and license key information.

**Support:** For technical support, licensing questions, or feature requests, contact us at jtplugin@ajl.vision

---

*This documentation covers version 1.0.0 of JT Magic Revolve. For the latest updates and features, please check the Autodesk App Store or our GitHub repository.*