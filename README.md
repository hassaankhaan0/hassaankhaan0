// ye apny taiqe ka ek hi object hai {singleton}
// object
 const JsUser= {
    name: "Hassaan",
    // is value ko kabhi bh dot . se access nh karskty.
    "full name": "Hassaan Naeem",
    [mySym]:"mykey1",
    age: 20,
    location: "karachi",
    email:"hassankhan@google.com",
    isLoggedIn: false,
    lastLoginDays:["Monday", "Saturday"]
 }
 
// symbol ko kese declare karty hn.
// const mySym = Symbol("key1")

 // is trha object declare karsakty hn.
// object 2 tariqon se declare hota hai.
// 1.object constructor.
   Object.create
// 2.object literal.
//  agar hum literals ki trha declare krty hn to singleton nhi bnta hai.
// or agar constructor se banaengy to humesha singleton banega.
// object ke andar keys or values ka chkkr hota hai.



// object ko access kese kia ja skta hai.
// 1.console.log(JsUser.email)
// 2.console.log(JsUser["email"])
// 3.console.log(JsUser["full name"])
// 4.console.log(JsUser[mySym])
    

// values ko change kese karty hn
JsUser.email = "hassan@chatgpt.com"
Object.freeze(JsUser)
JsUser.email = "hassan@microsoft.com"
console.log(JsUser);
