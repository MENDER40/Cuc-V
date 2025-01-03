local Fluent = loadstring(game:HttpGet("https://github.com/dawid-scripts/Fluent/releases/latest/download/main.lua"))()
local MarketplaceService = game:GetService("MarketplaceService")
local PlaceId = game.PlaceId
local ProductInfo = MarketplaceService:GetProductInfo(PlaceId)
local GameName = ProductInfo.Name

Fluent:Notify({ Title = "Script executado com sucesso", Content = "Você esta usando Mender_hub" })

local Window = Fluent:CreateWindow({
    Title = "Mender_hub",
    SubTitle = "-- " .. GameName,
    TabWidth = 102,
    Size = UDim2.fromOffset(450, 320),
    Acrylic = false,
    Theme = "Dark",
    MinimizeKey = Enum.KeyCode.LeftControl
})
local Tabs = {
    Main= Window:AddTab({ Title = "| Farm", Icon = "rbxassetid://18831424669" })
}

Window:SelectTab(1)
local AutoClick= Tabs.Main:AddToggle("Naruto", {Title = "Auto energy", Default = false})

AutoClick:OnChanged(function()
    while AutoClick.Value do
    --remote
    
game:GetService("ReplicatedStorage"):WaitForChild("Remotes"):WaitForChild("Energy"):WaitForChild("GainEnergy"):InvokeServer()
            wait(0)
           end
        end)
       
local Tabs = {
    Main= Window:AddTab({ Title = "| Hath", Icon = "rbxassetid://18831424669" })
}
Window:SelectTab(1)
local AutoClick= Tabs.Main:AddToggle("Naruto", {Title = "Naruto", Default = false})

AutoClick:OnChanged(function()
    while AutoClick.Value do
--remote
local args = {
    [1] = "Naruto",
    [2] = 1
}
game:GetService("ReplicatedStorage"):WaitForChild("Remotes"):WaitForChild("Eggs"):WaitForChild("Hatch"):InvokeServer(unpack(args))
        wait(0)
    end
end)
local AutoClick= Tabs.Main:AddToggle("OnePiece", {Title = "Onepiece ", Default = false})

AutoClick:OnChanged(function()
    while AutoClick.Value do
--remote
local args = {
    [1] = "OnePiece",
    [2] = 1
}

game:GetService("ReplicatedStorage"):WaitForChild("Remotes"):WaitForChild("Eggs"):WaitForChild("Hatch"):InvokeServer(unpack(args))

        wait(0)
    end
end)
local AutoClick= Tabs.Main:AddToggle("OnePiece", {Title = "DemonSlayer", Default = false})
AutoClick:OnChanged(function()
    while AutoClick.Value do
--remote
local args = {
    [1] = "DemonSlayer",
    [2] = 1
}
game:GetService("ReplicatedStorage"):WaitForChild("Remotes"):WaitForChild("Eggs"):WaitForChild("Hatch"):InvokeServer(unpack(args))
        wait(0)
    end
end)
local AutoClick= Tabs.Main:AddToggle("OnePiece", {Title = "Dragonball", Default = false})
AutoClick:OnChanged(function()
    while AutoClick.Value do
--remote
local args = {
    [1] = "DragonBall",
    [2] = 1
}
game:GetService("ReplicatedStorage"):WaitForChild("Remotes"):WaitForChild("Eggs"):WaitForChild("Hatch"):InvokeServer(unpack(args))
        wait(0)
    end
end)


Window:SelectTab(1)
local AutoClick= Tabs.Main:AddToggle("Naruto", {Title = "2xNaruto", Default = false})

AutoClick:OnChanged(function()
    while AutoClick.Value do
--remote
local args = {
    [1] = "Naruto",
    [2] = 2
}
game:GetService("ReplicatedStorage"):WaitForChild("Remotes"):WaitForChild("Eggs"):WaitForChild("Hatch"):InvokeServer(unpack(args))
        wait(0)
    end
end)
local AutoClick= Tabs.Main:AddToggle("OnePiece", {Title = "2xOnepiece ", Default = false})

AutoClick:OnChanged(function()
    while AutoClick.Value do
--remote
local args = {
    [1] = "OnePiece",
    [2] = 2
}

game:GetService("ReplicatedStorage"):WaitForChild("Remotes"):WaitForChild("Eggs"):WaitForChild("Hatch"):InvokeServer(unpack(args))

        wait(0)
    end
end)
local AutoClick= Tabs.Main:AddToggle("OnePiece", {Title = "2xDemonSlayer", Default = false})
AutoClick:OnChanged(function()
    while AutoClick.Value do
--remote
local args = {
    [1] = "DemonSlayer",
    [2] = 2
}
game:GetService("ReplicatedStorage"):WaitForChild("Remotes"):WaitForChild("Eggs"):WaitForChild("Hatch"):InvokeServer(unpack(args))
        wait(0)
    end
end)
local AutoClick= Tabs.Main:AddToggle("OnePiece", {Title = "2xDragonball", Default = false})
AutoClick:OnChanged(function()
    while AutoClick.Value do
--remote
local args = {
    [1] = "DragonBall",
    [2] = 2
}
game:GetService("ReplicatedStorage"):WaitForChild("Remotes"):WaitForChild("Eggs"):WaitForChild("Hatch"):InvokeServer(unpack(args))
        wait(0)
    end
end)

local AutoClick= Tabs.Main:AddToggle("Naruto", {Title = "3xNaruto", Default = false})

AutoClick:OnChanged(function()
    while AutoClick.Value do
--remote
local args = {
    [1] = "Naruto",
    [2] = 3
}
game:GetService("ReplicatedStorage"):WaitForChild("Remotes"):WaitForChild("Eggs"):WaitForChild("Hatch"):InvokeServer(unpack(args))
        wait(0)
    end
end)
local AutoClick= Tabs.Main:AddToggle("OnePiece", {Title = "3xOnepiece ", Default = false})

AutoClick:OnChanged(function()
    while AutoClick.Value do
--remote
local args = {
    [1] = "OnePiece",
    [2] = 3
}

game:GetService("ReplicatedStorage"):WaitForChild("Remotes"):WaitForChild("Eggs"):WaitForChild("Hatch"):InvokeServer(unpack(args))

        wait(0)
    end
end)
local AutoClick= Tabs.Main:AddToggle("OnePiece", {Title = "3xDemonSlayer", Default = false})
AutoClick:OnChanged(function()
    while AutoClick.Value do
--remote
local args = {
    [1] = "DemonSlayer",
    [2] = 3
}
game:GetService("ReplicatedStorage"):WaitForChild("Remotes"):WaitForChild("Eggs"):WaitForChild("Hatch"):InvokeServer(unpack(args))
        wait(0)
    end
end)
local AutoClick= Tabs.Main:AddToggle("OnePiece", {Title = "3xDragonball", Default = false})
AutoClick:OnChanged(function()
    while AutoClick.Value do
--remote
local args = {
    [1] = "DragonBall",
    [2] = 3
}
game:GetService("ReplicatedStorage"):WaitForChild("Remotes"):WaitForChild("Eggs"):WaitForChild("Hatch"):InvokeServer(unpack(args))
        wait(0)
    end
end)



local MainTab = Window:AddTab({ Title = "TELEPORT" })
Window:SelectTab(1)
MainTab:AddButton({
    Title = "Naruto",
    Callback = function()
--remote
  local args = {
    [1] = "Naruto"
}
game:GetService("ReplicatedStorage"):WaitForChild("Remotes"):WaitForChild("Islands"):WaitForChild("TeleportToIsland"):InvokeServer(unpack(args))
      print("TP“!")
    end
})

MainTab:AddButton({
    Title = "One piece",
    Callback = function()
--remote
  local args = {
    [1] = "OnePiece"
}

game:GetService("ReplicatedStorage"):WaitForChild("Remotes"):WaitForChild("Islands"):WaitForChild("TeleportToIsland"):InvokeServer(unpack(args))
  print("TP“!")
    end
})

MainTab:AddButton({
    Title = "DemonSlayer",
    Callback = function()
--remote
  local args = {
    [1] = "DemonSlayer"
}

game:GetService("ReplicatedStorage"):WaitForChild("Remotes"):WaitForChild("Islands"):WaitForChild("TeleportToIsland"):InvokeServer(unpack(args))
  print("TP“!")
    end
})

MainTab:AddButton({
    Title = "DragonBall",
    Callback = function()
--remote
  local args = {
    [1] = "DragonBall"
}

game:GetService("ReplicatedStorage"):WaitForChild("Remotes"):WaitForChild("Islands"):WaitForChild("TeleportToIsland"):InvokeServer(unpack(args))
  print("TP“!")
    end
})

local MainTab = Window:AddTab({ Title = "MISC" })

    local AutoClick= Tabs.Main:AddToggle("EquipBest", {Title = "Auto Equip best", Default = false})
AutoClick:OnChanged(function()
    while AutoClick.Value do
    --remote
    
game:GetService("ReplicatedStorage"):WaitForChild("Remotes"):WaitForChild("Pets"):WaitForChild("EquipBestPets"):FireServer()
            wait(10)
           end
        end)


local AutoClick= Tabs.Main:AddToggle("RankUp", {Title = "Auto rank up", Default = false})
AutoClick:OnChanged(function()
    while AutoClick.Value do
    --remote
game:GetService("ReplicatedStorage"):WaitForChild("Remotes"):WaitForChild("Rank"):WaitForChild("UpdateRank"):InvokeServer()
            wait(10)
           end
        end)

