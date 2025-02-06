Yeh React component Cards ke liye notes hain jo tumhare diye hue code ko explain karte hain.

1. Component ka Overview:
Yeh Cards ek functional React component hai.
Iska kaam hai ek list of products (jaise Coffee, Milk, Tea) ko display karna. Har product ka ek image, name, description, aur availability (in stock or out of stock) hota hai.
2. Data Array:
data ek array hai jisme objects hote hain. Har object ek product ko represent karta hai.
image: Product ka image URL.
name: Product ka naam (e.g., Coffee, Milk, Tea).
description: Product ka description.
instock: Boolean value (true ya false), jo bataata hai ki product stock me hai ya nahi.
3. Main Return Block:
return block mein humne ek div banaya hai jo poori screen ko cover karta hai (h-full w-full).
bg-gray-800 ka use karke background ko dark color diya gaya hai, aur flex justify-center items-center gap-2 se items ko center kiya gaya hai aur unke beech mein gap diya gaya hai.
4. Mapping over data:
data.map() function ka use karke hum har product ko loop kar rahe hain.
Har product ke liye ek div banaya gaya hai jisme:
Image: Har product ka image display hota hai.
Name and Description: Product ka name aur description text ke form mein display hota hai.
Button: Button ka label "In Stock" ya "Out of Stock" hota hai, jo instock property ke basis par set hota hai. Agar product stock mein hai to button ka background color bg-sky-700 hoga, aur agar product out of stock hai to bg-red-700 hoga.
5. Styling Classes:
h-[290px] w-[250px]: Har card ki height aur width define karta hai.
bg-white rounded-lg: Card ko white background aur rounded corners deta hai.
overflow-hidden: Image ko card ke andar properly fit karne ke liye overflow ko hide karta hai.
object-contain: Image ko container ke size ke hisaab se fit karta hai bina uski aspect ratio ko break kiye.
m-0, my-1.5, leading-tight: Text ka styling for margins, line height, and text spacing.
Button ke liye conditionally bg-sky-700 ya bg-red-700 class use hoti hai based on instock value.
6. Button Logic:
Button ka text conditional hai:
Agar instock true hai, to text "In Stock" dikhega.
Agar instock false hai, to text "Out of Stock" dikhega.
7. Output:
Is component ka output ek grid-style layout hota hai jisme products ka ek row ya column display hota hai, depending on the screen size.
Har card ek product ko represent karta hai, jisme image, name, description, aur availability button ke saath hoti hai.
