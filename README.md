# clerk-shadcn-theme
Easily synchronize your Clerk Sign-in and Sign-up components with your Shadcn styles using the provided CSS styles.

![Screenshot_4](https://github.com/stormynight9/clerk-shadcn-theme/assets/81434423/65804b03-cf66-43e0-ab19-9158c6ecf003)

 Just copy and paste the following code into your global CSS file, and you're good to go!
```css
.cl-formButtonPrimary {
    @apply inline-flex h-9 items-center justify-center whitespace-nowrap rounded-md bg-primary px-3 text-xs font-medium text-primary-foreground ring-offset-background transition-colors hover:bg-primary/90 focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50;
}

.cl-card,
.cl-socialButtonsBlockButton,
.cl-alert,
.cl-identityPreview,
.cl-phoneInputBox {
    @apply border border-input bg-background;
}

.cl-headerTitle,
.cl-socialButtonsBlockButtonText,
.cl-loading,
.cl-formFieldLabel,
.cl-formHeaderTitle,
.cl-selectButton__countryCode,
.cl-selectButton__countryCode p,
.cl-selectOption p,
.cl-selectOption div {
    @apply dark:text-foreground;
}

.cl-headerSubtitle,
.cl-dividerText,
.cl-footerActionText,
.cl-alertText,
.cl-formFieldInfoText,
.cl-formFieldSuccessText,
.cl-identityPreviewText,
.cl-formHeaderSubtitle {
    @apply text-muted-foreground;
}

.cl-dividerLine {
    @apply bg-border;
}

.cl-formFieldInput {
    @apply flex h-10 w-full rounded-md border border-input bg-background px-3 py-2 text-foreground ring-offset-background file:border-0 file:bg-transparent file:text-sm file:font-medium placeholder:text-muted-foreground focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:cursor-not-allowed disabled:opacity-50;
}

.cl-footerActionLink {
    @apply text-accent-foreground underline hover:text-accent-foreground/90;
}

.cl-otpCodeFieldInput {
    @apply border border-b-input text-foreground;
}

.cl-formResendCodeLink {
    @apply text-primary disabled:opacity-90;
}

.cl-selectSearchInput__countryCode {
    @apply flex h-10 w-full rounded-md border border-b border-input bg-background text-foreground ring-offset-background file:border-0 file:bg-transparent file:text-sm file:font-medium placeholder:text-muted-foreground focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:cursor-not-allowed disabled:opacity-50;
}

.cl-selectOptionsContainer__countryCode {
    @apply border border-input bg-background;
}

.cl-internal-icon {
    @apply text-foreground;
}

```
