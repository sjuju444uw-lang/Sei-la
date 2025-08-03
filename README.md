-- Farm automático de pushup, situp e punch
-- Insira em um LocalScript

local player = game.Players.LocalPlayer

local pushupEvent = game.ReplicatedStorage:FindFirstChild("pushup")
local situpEvent = game.ReplicatedStorage:FindFirstChild("situp")
local punchEvent = game.ReplicatedStorage:FindFirstChild("punch")

while true do
    if pushupEvent then
        pushupEvent:FireServer()
    end
    if situpEvent then
        situpEvent:FireServer()
    end
    if punchEvent then
        punchEvent:FireServer()
    end
    wait()
end
