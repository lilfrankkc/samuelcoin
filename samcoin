npx hardhat compile
const hre = require("hardhat");

async function main() {
  const USDToken = await hre.ethers.getContractFactory("USDToken");
  // Use the Chainlink ETH/USD price feed address for your network
  const priceFeedAddress = "0x5f4eC3Df9cbd43714FE2740f5E3616155c5b8419";
  const usdToken = await USDToken.deploy(priceFeedAddress);
  await usdToken.deployed();
  console.log("USDToken deployed to: - Untitled-1:11", usdToken.address);
}

main().catch((error) => {
  console.error(error);
  process.exitCode = 1;
});



 samuelcoin
