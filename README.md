local player = game.Players.LocalPlayer


local forcaEvent = game.ReplicatedStorage:FindFirstChild("Forca")
local durabilidadeEvent = game.ReplicatedStorage:FindFirstChild("Durabilidade")
local resistenciaEvent = game.ReplicatedStorage:FindFirstChild("Resistencia")

while true do
    -- Força
    if forcaEvent then
        forcaEvent:FireServer()
    end
    -- Durabilidade
    if durabilidadeEvent then
        durabilidadeEvent:FireServer()
    end
    -- Resistência
    if resistenciaEvent then
        resistenciaEvent:FireServer()
    end
    wait() -- Farma o mais rápido possível (sem delay)
end
