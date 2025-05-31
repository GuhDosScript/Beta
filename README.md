--carregar biblioteca
local Fluent = loadstring(game:HttpGet("https://github.com/dawid-scripts/Fluent/releases/latest/download/main.lua"))()

local Window = Fluent:CreateWindow({
    Title = "Guh's Hub " .. Fluent.Version,
    TabWidth = 160, Size = UDim2.fromOffset(580, 460), Theme = "Dark"
})

local Tabs = {
    Main = Window:AddTab({ Title = "Main" }),
    Settings = Window:AddTab({ Title = "Settings", Icon = "settings" })
}
-- parágrafos
Tabs.Main:AddParagraph({ Title = "Paragraph", Content = "Guh Gostozo" })
-- botões
Tabs.Main:AddButton({ Title = "Gerador", Callback = function() loadstring(game:HttpGet('https://raw.githubusercontent.com/ivannetta/ShitScripts/main/PathfindGens.lua,true'))() end })
