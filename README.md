local Fluent = loadstring(game:HttpGet("https://github.com/dawid-scripts/Fluent/releases/latest/download/main.lua"))()

--aviso ao executar
Fluent:Notify({ Discord= "Notification", Content = "https://discord.gg/3XvS5Kjr" })


local Window = Fluent:CreateWindow({
    Title = "potato hub" .. Fluent.Version,
    TabWidth = 160, Size = UDim2.fromOffset(580, 460), Theme = "Dark"
})

local Tabs = {
    Main = Window:AddTab({ Title = "credits" }),
    Settings = Window:AddTab({ Title = "Settings", Icon = "settings" })
}
--parágrafos
Tabs.Main:AddParagraph({ Title = "credits", Content = "credits:Theuzz" })

--botões
Tabs.Main:AddButton({ Title = "infinity yield", Callback = function()  
loadstring(game:HttpGet(('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'),true))()
end })
