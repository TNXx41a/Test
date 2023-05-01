local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("TITLE", "DarkTheme")
local Tab = Window:NewTab("Madu")
local Section = Tab:NewSection("Section Name")
Section:NewToggle("One", "ToggleInfo", function(state)
    if state then
        print("Toggle On")
        _G.JOJO = true
        while _G.JOJO do wait()
      game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-11.1798019, 137.500015, -511.367371, -1, 0, 0, 0, -1, 0, 0, 0, 1)
        end
        print("Toggle Off")
    end
end)
Section:NewButton("Stop", "ButtonInfo", function()
    print("Clicked")
     _G.JOJO = false
        while _G.JOJO do wait()
            end
end)
