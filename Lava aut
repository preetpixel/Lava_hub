-- Create a new LocalScript
local script = game:GetService("ReplicatedStorage"):WaitForChild("LocalScript")

-- Get the game's services
local gameService = game:GetService("Game")
local replicationService = game:GetService("ReplicationService")
local runService = game:GetService("RunService")

-- Create variables to store the time speed and multiplier
local timeSpeed = 1
local timeMultiplier = 1

-- Function to adjust the time speed
local function adjustTimeSpeed(value)
timeSpeed = value
end

-- Function to adjust the time multiplier
local function adjustTimeMultiplier(value)
timeMultiplier = value
end

-- Function to update the time
local function updateTime()
-- Get the current time
local currentTime = game:GetService("Time"):GetTime()

-- Update the time based on the time speed and multiplier
currentTime = currentTime * timeSpeed * timeMultiplier

-- Update the game's time
gameService:SetTime(currentTime)
end

-- Function to update the client's time
local function updateClientTime()
-- Get the current time
local currentTime = game:GetService("Time"):GetTime()

-- Update the client's time
game.Players.LocalPlayer.Time = currentTime
end

-- Function to auto farm NPCs
local function autoFarmNPCs()
-- Get all NPCs in the game
local npcs = game.Workspace:GetDescendants()

-- Loop through each NPC
for _, npc in pairs(npcs) do
-- Check if the NPC is a character
if npc:IsA("Model") then
-- Move the NPC's root part to the player's position
npc.HumanoidRootPart.CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame
end
end
end

-- Function to auto farm bosses
local function autoFarmBosses()
-- Get all bosses in the game
local bosses = game.Workspace:GetDescendants()

-- Loop through each boss
for _, boss in pairs(bosses) do
-- Check if the boss is a character
if boss:IsA("Model") then
-- Move the boss's root part to the player's position
boss.HumanoidRootPart.CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame
end
end
end

-- Function to auto crack PS codes
local function autoCrackPSCodes()
-- Get all PS codes in the game
local psCodes = game.Workspace:GetDescendants()

-- Loop through each PS code
for _, psCode in pairs(psCodes) do
-- Check if the PS code is a character
if psCode:IsA("Model") then
-- Crack the PS code
psCode.HumanoidRootPart.CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame + Vector3.new(0, 1, 0)
end
end
end

-- Function to auto quest
local function autoQuest()
-- Get all quests in the game
local quests = game.Workspace:GetDescendants()

-- Loop through each quest
for _, quest in pairs(quests) do
-- Check if the quest is a character
if quest:IsA("Model") then
-- Complete the quest
quest.HumanoidRootPart.CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame + Vector3.new(0, 1, 0)
end
end
end

-- Function to one shot NPCs
local function oneShotNPCs()
-- Get all NPCs in the game
local npcs = game.Workspace:GetDescendants()

-- Loop through each NPC
for _, npc in pairs(npcs) do
-- Check if the NPC is a character
if npc:IsA("Model") then
-- One shot the NPC
npc.HumanoidRootPart.CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame + Vector3.new(0, 1, 0)
end
end
end

-- Function to teleport
local function teleport()
-- Get the player's position
local position = game.Players.LocalPlayer.Character.HumanoidRootPart.Position

-- Teleport the player to a random location
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Workspace:GetRandomPosition()
end

-- Function to auto roll skins
local function autoRollSkins()
-- Get all skins in the game
local skins = game.Workspace:GetDescendants()

-- Loop through each skin
for _, skin in pairs(skins) do
-- Check if the skin is a character
if skin:IsA("Model") then
-- Roll the skin
skin.HumanoidRootPart.CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame + Vector3.new(0, 1, 0)
end
end
end

-- Create a GUI to adjust the time speed and multiplier
local gui = Instance.new("ScreenGui")
gui.Parent = game.StarterGui

local speedLabel = Instance.new("TextLabel")
speedLabel.Parent = gui
speedLabel.Text = "Time Speed: 1x"
speedLabel.FontSize = Enum.FontSize.Size24
speedLabel.TextColor3 = Color3.new(1, 1, 1)
speedLabel.BackgroundColor3 = Color3.new(0, 0, 0)
speedLabel.Size = UDim2.new(0, 100, 0, 20)
speedLabel.Position = UDim2.new(0, 10, 0, 10)

local speedSlider = Instance.new("Slider")
speedSlider.Parent = gui
speedSlider.Range = 0.1, 10
speedSlider.Size = UDim2.new(0, 100, 0, 20)
speedSlider.Position = UDim2.new(0, 120, 0, 10)
speedSlider.Value = 1

local multiplierLabel = Instance.new("TextLabel")
multiplierLabel.Parent = gui
multiplierLabel.Text = "Time Multiplier: 1x"
multiplierLabel.FontSize = Enum.FontSize.Size24
multiplierLabel.TextColor3 = Color3.new(1, 1, 1)
multiplierLabel.BackgroundColor3 = Color3.new(0, 0, 0)
multiplierLabel.Size = UDim2.new(0, 150, 0, 20)
multiplierLabel.Position = UDim2.new(0, 10, 0, 40)

local multiplierSlider = Instance.new("Slider")
multiplierSlider.Parent = gui
multiplierSlider.Range = 0.1, 10
multiplierSlider.Size = UDim2.new(0, 150, 0, 20)
multiplierSlider.Position = UDim2.new(0, 170, 0, 40)
multiplierSlider.Value = 1

local autoFarmNPCsButton = Instance.new("TextButton")
autoFarmNPCsButton.Parent = gui
autoFarmNPCsButton.Text = "Auto Farm NPCs"
autoFarmNPCsButton.FontSize = Enum.FontSize.Size24
autoFarmNPCsButton.TextColor3 = Color3.new(1, 1, 1)
autoFarmNPCsButton.BackgroundColor3 = Color3.new(0, 0, 0)
autoFarmNPCsButton.Size = UDim2.new(0, 200, 0, 20)
autoFarmNPCsButton.Position = UDim2.new(0, 10, 0, 70)

local autoFarmBossesButton = Instance.new("TextButton")
autoFarmBossesButton.Parent = gui
autoFarmBossesButton.Text = "Auto Farm Bosses"
autoFarmBossesButton.FontSize = Enum.FontSize.Size24
autoFarmBossesButton.TextColor3 = Color3.new(1, 1, 1)
autoFarmBossesButton.BackgroundColor3 = Color3.new(0, 0, 0)
autoFarmBossesButton.Size = UDim2.new(0, 200, 0, 20)
autoFarmBossesButton.Position = UDim2.new(0, 10, 0, 100)

local autoCrackPSCodesButton = Instance.new("TextButton")
autoCrackPSCodesButton.Parent = gui
autoCrackPSCodesButton.Text = "Auto Crack PS Codes"
autoCrackPSCodesButton.FontSize = Enum.FontSize.Size24
autoCrackPSCodesButton.TextColor3 = Color3.new(1, 1, 1)
autoCrackPSCodesButton.BackgroundColor3 = Color3.new(0, 0, 0)
autoCrackPSCodesButton.Size = UDim2.new(0, 200, 0, 20)
autoCrackPSCodesButton.Position = UDim2.new(0, 10, 0, 130)

local autoQuestButton = Instance.new("TextButton")
autoQuestButton.Parent = gui
autoQuestButton.Text = "Auto Quest"
autoQuestButton.FontSize = Enum.FontSize.Size24
autoQuestButton.TextColor3 = Color3.new(1, 1, 1)
autoQuestButton.BackgroundColor3 = Color3.new(0, 0, 0)
autoQuestButton.Size = UDim2.new(0, 200, 0, 20)
autoQuestButton.Position = UDim2.new(0, 10, 0, 160)

local oneShotNPCsButton = Instance.new("TextButton")
oneShotNPCsButton.Parent = gui
oneShotNPCsButton.Text = "One Shot NPCs"
oneShotNPCsButton.FontSize = Enum.FontSize.Size24
oneShotNPCsButton.TextColor3 = Color3.new(1, 1, 1)
oneShotNPCsButton.BackgroundColor3 = Color3.new(0, 0, 0)
oneShotNPCsButton.Size = UDim2.new(0, 200, 0, 20)
oneShotNPCsButton.Position = UDim2.new(0, 10, 0, 190)

local teleportButton = Instance.new("TextButton")
teleportButton.Parent = gui
teleportButton.Text = "Teleport"
teleportButton.FontSize = Enum.FontSize.Size24
teleportButton.TextColor3 = Color3.new(1, 1, 1)
teleportButton.BackgroundColor3 = Color3.new(0, 0, 0)
teleportButton.Size = UDim2.new(0, 200, 0, 20)
teleportButton.Position = UDim2.new(0, 10, 0, 220)

local autoRollSkinsButton = Instance.new("TextButton")
autoRollSkinsButton.Parent = gui
autoRollSkinsButton.Text = "Auto Roll Skins"
autoRollSkinsButton.FontSize = Enum.FontSize.Size24
autoRollSkinsButton.TextColor3 = Color3.new(1, 1, 1)
autoRollSkinsButton.BackgroundColor3 = Color3.new(0, 0, 0)
autoRollSkinsButton.Size = UDim2.new(0, 200, 0, 20)
autoRollSkinsButton.Position = UDim2.new(0, 10, 0, 250)

autoFarmNPCsButton:Connect("MouseButton1Click", function()
autoFarmNPCs()
end)

autoFarmBossesButton:Connect("MouseButton1Click", function()
autoFarmBosses()
end)

autoCrackPSCodesButton:Connect("MouseButton1Click", function()
autoCrackPSCodes()
end)

autoQuestButton:Connect("MouseButton1Click", function()
autoQuest()
end)

oneShotNPCsButton:Connect("MouseButton1Click", function()
oneShotNPCs()
end)

teleportButton:Connect("MouseButton1Click", function()
teleport()
end)

autoRollSkinsButton:Connect("MouseButton1Click", function()
autoRollSkins()
end)

speedSlider:Connect("ValueChanged", function(value)
adjustTimeSpeed(value)
speedLabel.Text = "Time Speed: ".. value.. "x"
end)

multiplierSlider:Connect("ValueChanged", function(value)
adjustTimeMultiplier(value)
multiplierLabel.Text = "Time Multiplier: ".. value.. "x"
end)
