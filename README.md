# task-2-ellipse-point-checker
Ellipse point checker 

A Java program that determines the position of points relative to an ellipse. Reads ellipse parameters and point coordinates from files, returns for each point: 0 (on boundary), 1 (inside), or 2 (outside).

Mathematical Foundation

The program uses the canonical ellipse equation to determine point positions:

((x - center_x) / radius_x)² + ((y - center_y) / radius_y)²

  -  Result ≈ 1.0: point on ellipse boundary (0)

  -  Result < 1.0: point inside ellipse (1)

  -  Result > 1.0: point outside ellipse (2)

For floating-point comparison, an epsilon value (1e-10) is used to account for calculation precision issues.
Error Handling

The program properly handles:

   - Missing files or incorrect paths

   - Invalid number formats in files
