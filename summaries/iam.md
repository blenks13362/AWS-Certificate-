# IAM (Identity and Access Management)

## 🔐 What is IAM?

IAM is AWS’s service for managing access to resources. It allows you to create users, groups, roles, and policies to control who can access what.

## 📌 Key Concepts

- **Users:** Individual identities with credentials.
- **Groups:** Collections of users sharing permissions.
- **Roles:** Identities with temporary credentials.
- **Policies:** JSON-based permissions documents.
- **Principals:** The entity (user, role, service) that performs actions.

## 🧠 Notes

- Always follow the **least privilege** principle.
- Use **MFA** on root and important users.
- Prefer roles over users for EC2 access.
- Inline policies = attached directly to entity  
  Managed policies = reusable and AWS-managed.

  📝 Questions to Expect on Exam
What’s the difference between a user and a role?

How to allow cross-account access?

How to enforce MFA?

## 🛠️ CLI Commands

```bash
aws iam list-users
aws iam create-user --user-name myUser
aws iam attach-user-policy --user-name myUser --policy-arn arn:aws:iam::aws:policy/ReadOnlyAccess


