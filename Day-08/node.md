# Flexbox
Turns a container into a flexible layout.

display: flex;
All direct children become flex items.

justify-content
Controls alignment along the main axis.

justify-content: center;
Values:

flex-start
center
flex-end
space-between
space-around
space-evenly
align-items
Controls alignment along the cross axis.

align-items: center;
Values:

stretch
center
flex-start
flex-end
gap
Adds spacing between flex items.

gap: 20px;
Example:

.menu {
  display: flex;
  gap: 15px;
}
Common Pattern
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 20px;
}
