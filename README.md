# NYS UNav Detector 🚀

The UNav Detector lets site admins check what implementation of the NYS UNav (Universal Navigation) headers and footers are in use on a site. It detects UNav elements on a page and whether it's using the recommended embedded script method or the outdated iframe or recreated methods. It also checks if a site is using HTTPS and belongs to a *.ny.gov domain (requirements of the new UNav).

The UNav Detector runs the following checks:

- Does the UNav exist, and if so, what version is in use (script, iframe, or undetermined)?
- Does the footer container exist, and if so, what version is in use (script, iframe, or undetermined)?
- Is the site using HTTPS?
- Does the site belong to a `*.ny.gov` domain?

> [!NOTE] 
> If the UNav Detector reports "🟥 Undetermined," but it looks like the site you're checking has a UNav at the top, it has probably been recreated manually. If you are unable to use the script embed on your site, please [request an exception via our UNav intake form](https://bit.ly/unav-intake).

## Usage

### How to Use

1. **Visit the UNav Detector:** [🔎 UNav Detector Tool](https://its-hcd.github.io/unav-detector/)
2. **Enter a URL.** Be sure to include the full URL. Best to visit a site and copy the URL directly from the browser. 
3. **Run the check.** If you get an error, the URL may be not fully formed or the site may be redirecting to a new page or blocking the detector.
4. **Review the Results.** Below is a list of potential results with more explanation:

### Results

- **UNav Header and Footer:** If this comes back as **🟢 Script**, you don't need to take any action — the script will update automatically. However, if this comes back as **🔷 Iframe** or **🟥 Undetermined**, you will need to update. If your site's platform does not allow for script embeds, please [request an exception via our UNav intake form](https://bit.ly/unav-intake).
- **HTTPS Check:** This is a straightforward check to see if the site is using a secure connection. If this comes back as **Not Using HTTPS (❌)**, your site will need to be updated to protect users from potential security risks before you can use the UNav.
- **NY.gov Domain Check:** Is this site a `*.ny.gov` site? If this comes back as **Not a NY.gov Domain (❌)**, you will not be able to use to NYS UNav.

## Contribution

Have a suggestion or improvement? Please feel free to [submit a pull request](https://github.com/ITS-HCD/unav-detector/pulls) or [open an issue](https://github.com/ITS-HCD/unav-detector/issues).

## Contact

For additional questions or support, please contact our Design System Team [via the UNav intake form](https://bit.ly/unav-intake).
