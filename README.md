# Samsung Galaxy A72 Linux

Install [postmarketOS](https://postmarketos.org/) on a [Samsung Galaxy A72](https://www.samsung.com/my/smartphones/galaxy-a/galaxy-a72-awesome-black-256gb-sm-a725fzkhxme/).

## References

- [postmarketOS - Samsung Galaxy A72](https://wiki.postmarketos.org/index.php?title=Samsung_Galaxy_A72_(samsung-a72q))
- [Python postmarketOS bootstrap package description](https://pypi.org/project/pmbootstrap/)

Create a project folder:

```sh
cd ~/ && mkdir Projects && cd Projects
```

Get the postmarketOS source code:

```sh
git clone https://github.com/jackvz/postmarketos-bootstrap.git
```

## Works

- USB Gadget mode
- Display (samsung,s6e3fc3-ams667ym01)
- GPU (FD618)
- Modem (works only with modemmanager. ofone doesn't seem to work)
- Wifi
- Bluetooth
- CPU (tlmm, clock controllers)
- UFS Storage
- SDHC (SDCard)
- IOMMU
- Battery (sm5714-fg)
- Charger (sm5714-charger)
- Touchscreen (stmfts_fts5cu56a)
- Some other things from sc7180.dtsi

## Broken

- Accelerometer & Gyroscope (lsm6dso)

## Bugs

- Display Brightness(Changing brightness causes artifacts)
- Modem sometimes can't start at boot.
