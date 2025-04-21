local FruitLocations = {
    ["Jungle"] = Vector3.new(-1337, 15, 448),
    ["Desert"] = Vector3.new(1094, 12, 4440),
    ["Snow Island"] = Vector3.new(1422, 55, -1323)
}

for name, position in pairs(FruitLocations) do
    local part = Instance.new("Part")
    part.Name = name .. "FruitSpawn"
    part.Position = position
    part.Size = Vector3.new(3, 3, 3)
    part.Anchored = true
    part.BrickColor = BrickColor.new("Bright red")
    part.Parent = game.Workspace
end
