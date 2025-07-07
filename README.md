**Tailwind Setup:	Used Tailwind CDN correctly **
Layout:	Designed a 2x2 grid using grid-cols-2 and grid-rows-2
Header:	Made a beautiful fixed header with flex, spacing, and z-10
Image Styling:	Used w-full, h-full, and object-cover to make images responsive and clean

**What Went Wrong + What I Fixed**
❌ Mistake-----------------------💡 Why it caused problems	--------------------------------------✅ How we fixed it
Used max-h-[50vh] & h-auto	--------Made images shrink unevenly and break the grid layout	 -----------Replaced with h-full to force them to fill their grid cell
Used min-h-screen	------------------Caused extra height and made scroll appear	----------------------Replaced with h-[calc(100vh-headerHeight)]
Didn't account for header height	--Grid was hidden under the fixed header	--------------------------Added pt-[80px] so grid content starts after the header

🧠 Lessons I've Learned (and Internalized!)
Concept	---------------------I Now Understand
grid-cols & grid-rows	-------How to build grid layouts
fixed header	---------------And how to give space below it using padding
h-full, object-cover	-------Controlling image sizing inside a container
calc(100vh - Xpx)	-----------How to subtract height and fit a layout on one screen
overflow-hidden	-------------Prevents scroll when you're sure all should fit
z-index, spacing, 
Tailwind utility classes-----Clean UI structure
