<h3 align="center">
    <samp>Hey, <sup><i>there!</i></sup>👋 welcome to my Github profile🧑
        take a look around, and clone away! 🔨</samp> 
</h3>
<h3 align="center" href="https://squidsync.com/">Visit my 📃webpage [here]</h3>
<p align="center">
  <img width="250" src="assets/200w.gif">
</p>

```lua
--*[[+ Cole.lua +]]*--
local Human = {}
Human.__index = Human
local Cole = { --> 🧑 @my profile!
    name = "Cole",
    career = "Programming 🖥️",
    pronouns = "he" or "him",
    employer = [[ Voldex ]]
}
Cole.__index = Cole
Cole.__type = "Male"
Cole.__call = "SquidSync"
setmetatable(Cole, Human) --> [Human -> Cole]
function Cole.About()
    return {
        profession = {
            name = "Game Developer",
            stack = {"Frontend", "Backend"}
        };
        interests = {
            "Enthusiast Web Developer",
            "Cat Owner (Ragdoll) 🐱 :3",
            "Coffee Lover"
        }
    }
end
function Cole.Family()
    local family = {}
    family.__index = Cole
    family.cat = {
        name = "Perl",
        breed = "Ragdoll",
        born = "10/24/21" --month/date/year
    }
    return family
end
function Cole:Wave(message): any?
    return string.format("%s says: Hey! 👋, %s!", self.name, message)
end
warn(Cole:Wave("Everybody")) --> "Cole says: Hey! 👋, Everybody!"
return setmetatable({}, Cole) -- @return <Singleton> [@Cole]
```