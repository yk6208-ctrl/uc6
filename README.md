public class OOPSBannerUC6 {

    // Method to generate pattern for letter O
    public static String[] getOPattern() {
        return new String[]{
                String.join("", "  *****  "),
                String.join("", " *     * "),
                String.join("", "*       *"),
                String.join("", "*       *"),
                String.join("", "*       *"),
                String.join("", " *     * "),
                String.join("", "  *****  ")
        };
    }

    // Method to generate pattern for letter P
    public static String[] getPPattern() {
        return new String[]{
                String.join("", " ******  "),
                String.join("", " *     * "),
                String.join("", " *     * "),
                String.join("", " ******  "),
                String.join("", " *       "),
                String.join("", " *       "),
                String.join("", " *       ")
        };
    }

    // Method to generate pattern for letter S
    public static String[] getSPattern() {
        return new String[]{
                String.join("", "  *****  "),
                String.join("", " *     * "),
                String.join("", " *       "),
                String.join("", "  *****  "),
                String.join("", "       * "),
                String.join("", " *     * "),
                String.join("", "  *****  ")
        };
    }

    public static void main(String[] args) {

        // Build banner lines using methods
        String[] o1 = getOPattern();
        String[] o2 = getOPattern();
        String[] p = getPPattern();
        String[] s = getSPattern();

        String[] bannerLines = new String[7];

        for (int i = 0; i < 7; i++) {
            bannerLines[i] = o1[i] + " " + o2[i] + " " + p[i] + " " + s[i];
        }

        // Print banner using enhanced for loop
        for (String line : bannerLines) {
            System.out.println(line);
        }
    }
}
