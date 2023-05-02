local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("Lenovo", "DarkTheme")
local Tab = Window:NewTab("inf")
local Section = Tab:NewSection("Skill Bom")
Section:NewButton("Z inf", "ButtonInfo", function()
    print("Clicked")
    local args = {
    [1] = Vector3.new(0.4539142847061157, -0.7665548324584961, -0.4542636275291443)
}

game:GetService("ReplicatedStorage").SkiIl:FireServer(unpack(args))
end)
Section:NewButton("N", "ButtonInfo", function()
    print("Clicked")
    game:GetService("ReplicatedStorage").Protect:FireServer()
end)
Section:NewButton("Punch", "ButtonInfo", function()
    print("Clicked")
    _G.Ora = true
    while _G.Ora do wait()
       game:GetService("ReplicatedStorage").Punch:FireServer() 
        end
end)
Section:NewButton("TaitanFast", "ButtonInfo", function()
    print("Clicked")
   game:GetService("ReplicatedStorage").Shift:FireServer()
end)
Section:NewButton("Stop", "ButtonInfo", function()
    print("Clicked")
    _G.Ora = false
    while _G.Ora do wait()
        end
end)
