
<p align="center">
  <img pointer-events="none" width="40%" height="40%" src="assets/200w.gif">
</p>
<h2 align="center">
    <samp color="rgb(3, 123, 252)"> Hey! Welcome to my Github profile.ð¨</samp> 
</h2>
<img src="assets/line.png">

```lua
--*[[+ Cole.lua +]]*--
local Human = {}
Human.__index = Human
local Cole = { --> ð§ @my profile!
    name = "Cole",
    career = "Programming ð¥ï¸",
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
            "Cat Owner (Ragdoll) ð± :3",
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
    return string.format("%s says: Hey! ð, %s!", self.name, message)
end
warn(Cole:Wave("Everybody")) --> "Cole says: Hey! ð, Everybody!"
return setmetatable({}, Cole) -- @return <Singleton> [@Cole]
```

<img src="assets/line.png">
<a href="https://squidsync.com/" style="text-align:center">Visit my webpageð [here]</a>