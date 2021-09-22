# Bitchcoin-Custom-ERC1155

This is a flattened contract based on OpenZepplin's [ERC1155PresetMinterPauserUpgradable.sol](https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/blob/master/contracts/token/ERC1155/presets/ERC1155PresetMinterPauserUpgradeable.sol).

Changes:
- Added `Owner` function. This modification was necessary to allow ownership from within NFT marketplaces.

# singleNFT-Custom-ERC721

This is a flattened contract based on OpenZepplin's [ERC721.sol](https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/token/ERC721/ERC721.sol).

Changes:
- Added `Owner` function. This modification was necessary to allow ownership from within NFT marketplaces.
- Added `Base_URI`, `Artist_Address`, `NFT_id` functions
- Added single mint in the main constructor. As this base contract does not implement mint/burn as external functions, this has the affect of creating an NFT contract for a single NFT, which can't be duplicated (minted) or destroyed.
- Removed `Symbol`
